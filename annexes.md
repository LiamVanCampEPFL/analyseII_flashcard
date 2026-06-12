# Annexes — Méthodes de calcul

---

## Tableau des ansatz pour $y_p$

> Pour $ay'' + by' + cy = g(x)$ à **coefficients constants**.

| Forme de $g(x)$ | Ansatz $p(x)$ | Condition |
|---|---|---|
| Polynôme de degré $n$ | polynôme de degré $n$ | $c \neq 0$ |
| Polynôme de degré $n$ | polynôme de degré $n+1$ | $c = 0,\ b \neq 0$ |
| Polynôme de degré $n$ | polynôme de degré $n+2$ | $b = c = 0$ |
| $g(x) = \lambda e^{\kappa x}$ | $p(x) = \alpha e^{\kappa x}$ | cas standard |
| $g(x) = \lambda e^{\kappa x}$ | $p(x) = \alpha x e^{\kappa x}$ | si $\kappa$ racine simple |
| $g(x) = \lambda e^{\kappa x}$ | $p(x) = \alpha x^2 e^{\kappa x}$ | si $\kappa$ racine double |
| $g(x) = \lambda\sin(\omega x)$ | $p(x) = \alpha\sin(\omega x) + \beta\cos(\omega x)$ | cas standard |
| $g(x) = \lambda\cos(\omega x)$ | $p(x) = \alpha\sin(\omega x) + \beta\cos(\omega x)$ | cas standard |
| $g(x) = e^{\kappa x}(\lambda\sin(\omega x) + \mu\cos(\omega x))$ | $p(x) = e^{\kappa x}(\alpha\sin(\omega x) + \beta\cos(\omega x))$ | cas standard |
| $g(x) = e^{\kappa x}(\lambda\sin(\omega x) + \mu\cos(\omega x))$ | $p(x) = xe^{\kappa x}(\alpha\sin(\omega x) + \beta\cos(\omega x))$ | si $\kappa \pm i\omega$ racine |
| Combinaison linéaire | combinaison linéaire des $p$ correspondants | superposition |

### Règle générale

1. Identifier la forme de $g(x)$ dans le tableau
2. Poser $p(x)$ selon l'ansatz correspondant
3. Substituer $p(x)$ dans l'équation et identifier les coefficients
4. Si plusieurs termes dans $g(x)$ → superposer les $y_p$

> Si l'ansatz est déjà solution de l'homogène, multiplier par $x$ (ou $x^2$ si racine double).

---

## Suites dans ℝ — limites et critères

### Définition de convergence

$(a_n)$ converge vers $a \in \mathbb{R}$ si :
$$\forall \varepsilon > 0,\ \exists n_0 \in \mathbb{N} \text{ tel que } \forall n \geq n_0,\ |a_n - a| \leq \varepsilon$$

### Suites usuelles et leur comportement

| Suite $a_n$ | Limite | Monotonie | Bornée |
|---|---|---|---|
| $\dfrac{1}{n}$ | $0$ | décrois. stricte | oui, $\in (0,1]$ |
| $\dfrac{1}{n^p}$, $p > 0$ | $0$ | décrois. stricte | oui |
| $q^n$, $\|q\| < 1$ | $0$ | — | oui |
| $q^n$, $q > 1$ | $+\infty$ | crois. stricte | non |
| $q^n$, $q = -1$ | diverge | alternée | oui |
| $\sqrt[n]{n}$ | $1$ | décrois. pour $n \geq 3$ | oui |
| $\sqrt[n]{c}$, $c > 0$ | $1$ | — | oui |
| $\left(1 + \dfrac{1}{n}\right)^n$ | $e$ | crois. stricte | oui |
| $\left(1 + \dfrac{x}{n}\right)^n$ | $e^x$ | — | oui |
| $\dfrac{n^k}{q^n}$, $q > 1$ | $0$ | — | oui |
| $\dfrac{q^n}{n!}$ | $0$ | — | oui |
| $\dfrac{\ln n}{n}$ | $0$ | décrois. pour $n \geq 3$ | oui |

> **Hiérarchie des infinis :** $\ln n \ll n^p \ll q^n \ll n! \ll n^n$

### Méthodes pour trouver/montrer une limite

**Méthode 1 : Suite monotone et bornée**
Toute suite monotone et bornée est convergente.
- Croissante + majorée → converge
- Décroissante + minorée → converge

**Méthode 2 : Théorème des gendarmes**
Si $b_n \leq a_n \leq c_n$ et $\lim b_n = \lim c_n = L$, alors $\lim a_n = L$.

**Méthode 3 : Opérations sur les limites**
Si $\lim a_n = a$ et $\lim b_n = b$ :
$$\lim(a_n + b_n) = a+b, \quad \lim(a_n b_n) = ab, \quad \lim\frac{a_n}{b_n} = \frac{a}{b}\ (b \neq 0)$$

**Méthode 4 : Comparaison avec suites usuelles**
$$\frac{1}{n} \to 0, \quad q^n \to 0 \text{ si } |q|<1, \quad \sqrt[n]{n} \to 1$$

**Méthode 5 : Définition directe**
Montrer que $|a_n - a| \leq f(n)$ avec $\lim f(n) = 0$.

**Règle de d'Alembert pour les suites**
Si $\lim \left|\dfrac{a_{n+1}}{a_n}\right| = s$ :
- $s < 1$ → $\lim a_n = 0$
- $s > 1$ → $(a_n)$ diverge
- $s = 1$ → pas de conclusion

### Suite de Cauchy

$(a_n)$ est de Cauchy si $\forall \varepsilon > 0,\ \exists n_0$ tel que $\forall n,m \geq n_0,\ |a_n - a_m| \leq \varepsilon$.

Dans $\mathbb{R}$ : $(a_n)$ converge $\iff$ $(a_n)$ est de Cauchy.

### Bolzano-Weierstrass

Toute suite réelle **bornée** admet une **sous-suite convergente**.

---

## Limites de fonctions dans ℝ

### Définition ($\varepsilon$-$\delta$)

$$\lim_{x \to a} f(x) = \ell \iff \forall \varepsilon > 0,\ \exists \delta > 0 \text{ tel que } 0 < |x-a| < \delta \Rightarrow |f(x) - \ell| < \varepsilon$$

> La valeur $f(a)$ n'intervient pas — $f$ peut ne pas être définie en $a$.

### Existence de la limite

$$\lim_{x \to a} f(x) \text{ existe} \iff \lim_{x \to a^-} f(x) = \lim_{x \to a^+} f(x)$$

### Limites classiques ($x \to 0$)

$$\lim_{x \to 0} \cos(x) = 1, \qquad \lim_{x \to 0} \frac{\sin(x)}{x} = 1, \qquad \lim_{x \to 0} \frac{1 - \cos(x)}{x^2} = \frac{1}{2}$$

### Théorème des deux gendarmes

Si $g(x) \leq f(x) \leq h(x)$ au voisinage de $a$ et $\lim g = \lim h = L$, alors $\lim f = L$.

### Continuité en un point

$f$ est continue en $a$ $\iff$ $\lim_{x \to a} f(x) = f(a)$, c'est-à-dire :
1. $f(a)$ est définie
2. La limite existe
3. La limite vaut $f(a)$

### Prolongement par continuité

Si $f$ n'est pas définie en $a$ mais $\ell = \lim_{x \to a} f(x)$ existe et est finie, on peut poser $\tilde{f}(a) = \ell$ → $\tilde{f}$ est continue en $a$.

---

## Intégration par parties

$$\int v \cdot w' \, dx = v \cdot w - \int v' \cdot w \, dx$$

**Astuce $\sin/\cos \times \exp$ :** intégrer par parties deux fois → l'intégrale réapparaît → isoler algébriquement :

$$\left(1 + \frac{\omega^2}{a^2}\right) I = \cdots \implies I = \frac{e^{ax}}{a^2 + \omega^2}(a\sin(\omega x) - \omega\cos(\omega x))$$
