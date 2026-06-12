# Propriétés — Vrai / Faux

> Format : ✅ Vrai | ❌ Faux | ⚠️ Dépend des conditions
> Utilisation : cache la réponse et teste-toi.

---

## Ch. 0-2 — EDO 1er ordre

| Propriété | Réponse |
|---|---|
| Toute EDO séparable est aussi linéaire | ❌ (séparable ≠ linéaire en général) |
| $y' = f(x)g(y)$ est séparable | ✅ |
| Une EDO linéaire a toujours une solution unique si les coefficients sont continus et une CI est donnée | ✅ (Cauchy-Lipschitz) |
| $y \equiv 0$ est toujours solution d'une EDO linéaire homogène | ✅ |
| La solution générale d'une EDO linéaire est $y = y_{\text{hom}} + y_p$ | ✅ |
| Pour Bernoulli $n=1$, la substitution $z = y^{-(n-1)}$ est nécessaire | ❌ ($n=1$ → déjà linéaire) |
| $y \equiv 0$ est solution de Bernoulli pour tout $n$ | ✅ |
| L'équation $y' = y/x + (y/x)^2$ est de type Euler homogène | ✅ ($f$ dépend de $y/x$) |
| Une EDO de Bernoulli avec $n=2$ a toujours 4 familles de solutions maximales | ⚠️ (dépend de $z = y^{-1}$ et ses zéros) |

---

## Ch. 2 — EDO 2nd ordre

| Propriété | Réponse |
|---|---|
| Si $y_1, y_2$ sont solutions de $L[y]=0$ alors $C_1y_1 + C_2y_2$ aussi | ✅ (principe de superposition) |
| Le Wronskien $W[y_1,y_2] \neq 0$ implique $y_1, y_2$ linéairement indépendants | ✅ |
| $W[y_1,y_2] = 0$ implique $y_1, y_2$ linéairement dépendants | ✅ (si coefficients continus) |
| Pour $\Delta < 0$, les solutions sont réelles | ✅ (on prend parties réelle/imaginaire) |
| Pour $\Delta = 0$, la solution générale est $(C_1 + C_2 x)e^{\lambda x}$ | ✅ |
| L'ansatz s'applique aux EDO à coefficients **non constants** | ❌ (coefficients constants seulement) |
| Si $\kappa$ est racine simple du pol. caract., l'ansatz $\alpha e^{\kappa x}$ reste valable | ❌ (il faut multiplier par $x$) |
| La variation des constantes fonctionne pour tout $g(x)$ | ✅ |
| Pour Euler-Cauchy $x^2y''+bxy'+cy=0$, on substitue $t = \ln x$ | ✅ |
| Après substitution Euler-Cauchy, on obtient une EDO à coefficients constants | ✅ |

---

## Ch. 3.1 — Produit scalaire et norme

| Propriété | Réponse |
|---|---|
| $\langle x, y\rangle = \langle y, x\rangle$ | ✅ (symétrie) |
| $\langle x, x\rangle \geq 0$ et $= 0 \iff x = 0$ | ✅ (positivité) |
| $\langle x, \alpha y + \beta z\rangle = \alpha\langle x,y\rangle + \beta\langle x,z\rangle$ | ✅ (bilinéarité) |
| $|\langle x,y\rangle| \leq \|x\| \cdot \|y\|$ | ✅ (Cauchy-Schwarz) |
| $\langle x,y\rangle = 0 \implies x = 0$ ou $y = 0$ | ❌ ($x \perp y$ mais aucun n'est forcément nul) |
| Si $\langle x,y\rangle = 0$ alors $\|x+y\|^2 = \|x\|^2 + \|y\|^2$ | ✅ (Pythagore) |
| $\|x+y\| \leq \|x\| + \|y\|$ | ✅ (inégalité triangulaire) |
| $\langle x,y\rangle = \|x\|\|y\|\cos\theta$ permet de calculer l'angle entre deux vecteurs | ✅ |
| $\|x+y\|^2 + \|x-y\|^2 = 2\|x\|^2 + 2\|y\|^2$ (loi du parallélogramme) | ✅ |

---

## Ch. 3.2 — Topologie

| Propriété | Réponse |
|---|---|
| $B(a,r)$ est un ensemble ouvert | ✅ |
| $\bar{B}(a,r)$ est un ensemble fermé | ✅ |
| Tout ensemble ouvert est aussi fermé | ❌ (sauf $\emptyset$ et $\mathbb{R}^n$) |
| $\mathbb{R}^n$ est à la fois ouvert et fermé | ✅ |
| $\emptyset$ est à la fois ouvert et fermé | ✅ |
| $[0,1)$ est ni ouvert ni fermé dans $\mathbb{R}$ | ✅ |
| L'union quelconque d'ouverts est ouverte | ✅ |
| L'intersection quelconque d'ouverts est ouverte | ❌ (finie seulement) |
| L'union finie de fermés est fermée | ✅ |
| L'union infinie de fermés est fermée | ❌ (pas forcément) |
| $U \setminus C$ est ouvert si $U$ ouvert et $C$ fermé | ✅ |
| $\partial S = \partial S^c$ | ✅ (la frontière est la même) |
| $S$ est ouvert $\iff S = \mathring{S}$ | ✅ |
| $S$ est fermé $\iff \partial S \subset S$ | ✅ |
| $\bar{S} = \mathring{S} \cup \partial S$ | ✅ |
| Si $S$ est fermé alors $S^c$ est ouvert | ✅ (définition) |
| $f(x) < c$ définit toujours un ensemble ouvert | ⚠️ (si $f$ continue, oui) |
| $f(x) \leq c$ définit toujours un ensemble fermé | ⚠️ (si $f$ continue, oui) |

---

## Ch. 3.3 — Suites dans ℝⁿ

| Propriété | Réponse |
|---|---|
| $(x_k) \to x$ dans $\mathbb{R}^n$ $\iff$ chaque coordonnée converge | ✅ |
| Une suite convergente est forcément bornée | ✅ |
| Une suite bornée est forcément convergente | ❌ (ex : $(-1)^k$ borné mais diverge) |
| Une suite bornée admet une sous-suite convergente | ✅ (Bolzano-Weierstrass) |
| Si $(x_k) \subset C$ compact, la sous-suite convergente a sa limite dans $C$ | ✅ ($C$ fermé → limite dans $C$) |
| Toute suite de Cauchy dans $\mathbb{R}^n$ est convergente | ✅ ($\mathbb{R}^n$ est complet) |
| $\lim(x_k + y_k) = \lim x_k + \lim y_k$ si les deux convergent | ✅ |
| $\lim\langle x_k, y_k\rangle = \langle \lim x_k, \lim y_k\rangle$ | ✅ (produit scalaire continu) |
| $\lim \|\,x_k\| = \|\lim x_k\|$ | ✅ (norme continue) |
| Si $(x_k) \subset F$ fermé et $x_k \to x$, alors $x \in F$ | ✅ (définition du fermé) |
| $x \in \bar{S}$ $\iff$ il existe une suite $(x_k) \subset S$ avec $x_k \to x$ | ✅ (caract. séquentielle) |
| $S$ fermé $\iff$ toute suite de $S$ qui converge a sa limite dans $S$ | ✅ (équivalent à $S = \bar{S}$) |

---

## Ch. 3.4 — Courbes paramétriques

| Propriété | Réponse |
|---|---|
| $f : I \to \mathbb{R}^n$ est continue en $t_0$ $\iff$ chaque composante $f_1, \dots, f_n$ est continue en $t_0$ | ✅ (critère composante par composante) |

---

## Ch. 4.3 — Fonctions de plusieurs variables : extrema et TFI

### Points stationnaires \& extrema locaux

| Propriété | Réponse |
|---|---|
| $\nabla f(\mathbf{a}) = \mathbf{0} \implies \mathbf{a}$ est un extremum local | ❌ (peut être point selle) |
| $\mathbf{a}$ extremum local et $f$ diff. en $\mathbf{a}$ $\implies \nabla f(\mathbf{a}) = \mathbf{0}$ | ✅ (Prop. 4.4) |
| Un extremum local peut exister sans que $f$ soit différentiable en $\mathbf{a}$ | ✅ (ex. coin, bord $\partial E$) |
| Les points stationnaires sont les seuls candidats à un extremum local | ❌ (aussi : $f$ non diff. et $\mathbf{a} \in \partial E$) |
| $\nabla f(\mathbf{a}) = \mathbf{0}$ et $f$ différentiable $\implies$ extremum local | ❌ (nécessaire, non suffisant) |

### Point selle (Déf. 4.24)

| Propriété | Réponse |
|---|---|
| $\mathbf{a}$ point selle $\implies \nabla f(\mathbf{a}) = \mathbf{0}$ | ✅ (par définition) |
| $\mathbf{a}$ point selle $\implies \mathbf{a}$ extremum local | ❌ (par définition : ce n'est **pas** un extremum) |
| Au point selle, le plan tangent $z = \mathcal{P}_1(\mathbf{x})$ est horizontal | ✅ |
| $f(x,y) = x^2 - y^2$ admet un point selle en $(0,0)$ | ✅ ($D = -4 < 0$) |
| $f(x,y) = x^3 - 3xy^2$ (monkey saddle) admet un extremum en $(0,0)$ | ❌ (point selle dégénéré) |

### Test de la dérivée seconde — cas $n=2$ (Théorème 4.13)

Rappel : $D = \det(\mathrm{Hess}(f)(a,b)) = \dfrac{\partial^2 f}{\partial x^2}\dfrac{\partial^2 f}{\partial y^2} - \left(\dfrac{\partial^2 f}{\partial x \partial y}\right)^2$

| Propriété | Réponse |
|---|---|
| $D > 0$ et $\dfrac{\partial^2 f}{\partial x^2}(a,b) > 0 \implies$ minimum local en $(a,b)$ | ✅ |
| $D > 0$ et $\dfrac{\partial^2 f}{\partial x^2}(a,b) < 0 \implies$ maximum local en $(a,b)$ | ✅ |
| $D < 0 \implies$ point selle en $(a,b)$ | ✅ |
| $D = 0 \implies$ point selle en $(a,b)$ | ❌ (test **non concluant**) |
| $D > 0 \implies \dfrac{\partial^2 f}{\partial x^2}$ et $\dfrac{\partial^2 f}{\partial y^2}$ ont le même signe | ✅ |
| $\det(\mathrm{Hess}(f)(\mathbf{a})) > 0$ suffit pour conclure à un extremum si $n \geq 3$ | ❌ (il faut toutes les $\lambda_i$) |
| $\lambda_1 \lambda_2 > 0 \implies$ extremum local ($n=2$) | ✅ (même signe $\implies$ $\mathrm{Hess}$ définie) |
| $\lambda_1 + \lambda_2 + \lambda_3 = 2,\ \lambda_1\lambda_2\lambda_3 = -1 \implies$ pas d'extremum | ✅ (produit $< 0 \implies$ signes mixtes $\implies$ selle) |
| $\mathrm{Hess}(f)(\mathbf{a}) = \mathrm{diag}(1,2,3) \implies$ minimum local | ✅ (tous $\lambda_i > 0$) |

### Test dérivée seconde — cas général (Théorème 4.14)

$\lambda_1,\ldots,\lambda_n$ désignent les valeurs propres de $\mathrm{Hess}(f)(\mathbf{a})$.

| Propriété | Réponse |
|---|---|
| $\forall i,\ \lambda_i > 0 \implies$ minimum local en $\mathbf{a}$ | ✅ ($\mathrm{Hess}$ définie positive) |
| $\forall i,\ \lambda_i < 0 \implies$ maximum local en $\mathbf{a}$ | ✅ ($\mathrm{Hess}$ définie négative) |
| $\forall i,\ \lambda_i \neq 0$ et signes mixtes $\implies$ point selle en $\mathbf{a}$ | ✅ ($\mathrm{Hess}$ indéfinie) |
| $\exists\, i : \lambda_i = 0 \implies$ test non concluant | ✅ |
| Pour $\mathrm{Hess}$ diagonale, les $\lambda_i$ sont les entrées diagonales | ✅ |

### TFI — Théorème des fonctions implicites (Théorème 4.15)

| Propriété | Réponse |
|---|---|
| $F(\mathbf{a}) = c$ et $\dfrac{\partial F}{\partial x_n}(\mathbf{a}) \neq 0 \implies x_n = f(x_1,\ldots,x_{n-1})$ existe localement | ✅ (Thm. 4.15) |
| $\dfrac{\partial F}{\partial x_n}(\mathbf{a}) = 0 \implies x_n$ non défini implicitement | ❌ (condition suffisante, pas nécessaire — TFI ne s'applique pas, mais $f$ peut quand même exister) |
| Le TFI fournit la formule explicite de $f$ | ❌ (garantit seulement l'**existence** locale) |
| Si TFI s'applique, on peut calculer $\dfrac{\partial f}{\partial x_i}$ par différentiation implicite | ✅ (§4.3.19) |
| $F(x,y) = x^2+y^2$, $\dfrac{\partial F}{\partial y}(1,0) = 0 \implies y$ non défini implicitement près de $(1,0)$ | ✅ ($y = \pm\sqrt{1-x^2}$ : pas unique) |

---

## Ch. 5 — Fonctions vectorielles $f : \mathbb{R}^n \to \mathbb{R}^m$

### Hiérarchie et implications

| Propriété | Réponse |
|---|---|
| $f \in C^1 \implies f$ différentiable | ✅ |
| $f$ différentiable $\implies f \in C^1$ | ❌ |
| $f$ différentiable $\implies f$ continue | ✅ |
| $f$ continue $\implies f$ différentiable | ❌ |
| $f$ différentiable $\implies \partial f_i/\partial x_j$ existent toutes | ✅ |
| $\partial f_i/\partial x_j$ existent toutes $\implies f$ différentiable | ❌ |
| $\partial f_i/\partial x_j$ existent toutes $\implies f$ continue | ❌ |

### Critère composante par composante

| Propriété | Réponse |
|---|---|
| $f$ continue en $\mathbf{a}$ $\iff$ chaque $f_i$ continue en $\mathbf{a}$ | ✅ (Prop. 5.4) |
| $f$ différentiable en $\mathbf{a}$ $\iff$ chaque $f_i$ différentiable en $\mathbf{a}$ | ✅ (Prop. 5.4) |
| $f \in C^1(E)$ $\iff$ chaque $f_i \in C^1(E)$ | ✅ (Prop. 5.4) |
| $\lim_{\mathbf{x}\to\mathbf{a}} f(\mathbf{x}) = \mathbf{b}$ $\iff$ $\lim f_i(\mathbf{x}) = b_i$ pour tout $i$ | ✅ |

### Matrice Jacobienne

| Propriété | Réponse |
|---|---|
| $J_f(\mathbf{a}) \in \mathbb{R}^{m \times n}$ (m lignes, n colonnes) | ✅ |
| La ligne $i$ de $J_f(\mathbf{a})$ est $\nabla f_i(\mathbf{a})^\top$ | ✅ |
| Si $f : \mathbb{R}^n \to \mathbb{R}$ (scalaire), $J_f(\mathbf{a}) = \nabla f(\mathbf{a})^\top$ (vecteur ligne) | ✅ |
| Si $f$ différentiable, $\nabla_\mathbf{v} f(\mathbf{a}) = J_f(\mathbf{a}) \cdot \mathbf{v}$ avec $\|\mathbf{v}\|=1$ | ✅ |
| La Jacobienne existe même si $f$ n'est pas différentiable | ✅ (les dérivées partielles peuvent exister sans diff.) |
| $f$ différentiable $\implies$ la Jacobienne est l'unique application linéaire $L_\mathbf{a}$ | ✅ |

### Chain Rule N°2 (Thm 5.2)

Pour $g : \mathbb{R}^n \to \mathbb{R}^p$ et $f : \mathbb{R}^p \to \mathbb{R}^q$ :

| Propriété | Réponse |
|---|---|
| $J_{f \circ g}(\mathbf{a}) = J_f(g(\mathbf{a})) \cdot J_g(\mathbf{a})$ | ✅ (si $g$ diff. en $\mathbf{a}$, $f$ diff. en $g(\mathbf{a})$) |
| $J_{f \circ g}(\mathbf{a})$ est de taille $q \times n$ | ✅ |
| L'ordre de multiplication est $J_f \cdot J_g$ (pas $J_g \cdot J_f$) | ✅ (produit matriciel non commutatif) |
| Si $f$ scalaire ($q=1$) : $\nabla(f\circ g)(\mathbf{a}) = J_g(\mathbf{a})^\top \cdot \nabla f(g(\mathbf{a}))$ | ✅ |
| La Chain Rule s'applique même si les dimensions intermédiaires diffèrent | ✅ (tant que les types correspondent) |

### Lagrange multi-contraintes (Thm 5.3)

| Propriété | Réponse |
|---|---|
| Condition nécessaire : $\nabla f(\mathbf{a}) = \sum_i \lambda_i \nabla g_i(\mathbf{a})$ | ✅ (si les $\nabla g_i$ sont linéairement indépendants) |
| Les $\lambda_i$ (multiplicateurs) sont des extrema de $f$ | ❌ (ce sont des scalaires auxiliaires) |
| Si $\nabla g_1(\mathbf{a}), \ldots, \nabla g_k(\mathbf{a})$ sont linéairement dépendants, le Thm. 5.3 s'applique encore | ❌ (hypothèse nécessaire : indépendance linéaire) |
| On a $n + k$ équations pour $n + k$ inconnues ($\mathbf{x}$ et $\boldsymbol{\lambda}$) | ✅ |
| Lagrange garantit que les points candidats sont des extrema | ❌ (condition nécessaire, non suffisante — il faut comparer les valeurs) |
| Si le domaine contraint est compact, il existe un max et un min globaux | ✅ (Weierstrass) |

---

## Ch. 6 — Intégrales multiples

### Fubini & ordre d'intégration

| Propriété | Réponse |
|---|---|
| On peut toujours échanger l'ordre d'intégration | ❌ (valable si $f$ continue sur le domaine, ou par Fubini si $f \geq 0$) |
| $\int_a^b\!\int_c^d f(x,y)\,dy\,dx = \int_c^d\!\int_a^b f(x,y)\,dx\,dy$ sur un rectangle | ✅ (si $f$ continue) |
| Changer l'ordre ne change pas la valeur de l'intégrale | ✅ (sous les hypothèses de Fubini) |
| Si $\int_0^1\!\int_x^1 f(y)\,dy\,dx$, on peut swap en $\int_0^1\!\int_0^y f(y)\,dx\,dy$ | ✅ (même domaine triangulaire) |

### Changement de variables

| Propriété | Réponse |
|---|---|
| $dx\,dy = \lvert\det J_\Phi\rvert\,du\,dv$ | ✅ |
| Le déterminant de la Jacobienne peut être négatif, c'est grave | ❌ (on prend la valeur absolue) |
| $J_\Phi$ est la matrice des dérivées partielles de $(x,y)$ par rapport à $(u,v)$ | ✅ |
| Si $\Phi$ n'est pas bijective sur l'intérieur, le changement de variables est invalide | ✅ |
| Pour des coordonnées polaires, $\det J_\Phi = r$ | ✅ ($\partial(x,y)/\partial(r,\theta) = r$) |

### Coordonnées polaires

| Propriété | Réponse |
|---|---|
| $\iint_D f\,dx\,dy = \iint_E f(r\cos\theta, r\sin\theta)\,dr\,d\theta$ | ❌ (il manque le facteur $r$) |
| $\iint_D f\,dx\,dy = \iint_E f(r\cos\theta, r\sin\theta)\cdot r\,dr\,d\theta$ | ✅ |
| $\iint_E g(r)h(\theta)\,r\,dr\,d\theta = \bigl(\int g(r)\,r\,dr\bigr)\bigl(\int h(\theta)\,d\theta\bigr)$ si les bornes dépendent de $\theta$ | ❌ (séparation valide **seulement** si toutes les bornes sont constantes) |
| $r = a\cos\theta$ est un cercle en coordonnées cartésiennes | ✅ (cercle centré en $(a/2,0)$, rayon $a/2$) |
| Sur $x^2+y^2 \leq R^2$, les bornes polaires sont $r \in [0,R]$, $\theta \in [0,2\pi]$ | ✅ |
| $x \geq 0$ en polaires correspond à $\theta \in [-\pi/2, \pi/2]$ | ✅ ($\cos\theta \geq 0$) |

### Applications

| Propriété | Réponse |
|---|---|
| $\iint_D 1\,dx\,dy = \text{Aire}(D)$ | ✅ |
| $\bar{f} = \iint_D f\,dx\,dy$ (valeur moyenne) | ❌ (il faut diviser par $\text{Aire}(D)$) |
| $M = \iint_D \delta\,dx\,dy$ (masse avec densité $\delta$) | ✅ |
| $\bar{x} = \frac{1}{M}\iint_D x\,\delta\,dx\,dy$ | ✅ |
| Si $D$ symétrique / axe $y$ et $\delta(-x,y)=\delta(x,y)$, alors $\bar{x}=0$ | ✅ (intégrande impaire $\Rightarrow$ intégrale nulle) |
| Si $D$ symétrique / axe $y$ et $\delta$ quelconque, alors $\bar{x}=0$ | ❌ (faut aussi $\delta$ paire en $x$) |

---

## Ch. 7 — Intégrales triples

### Fubini & ordre d'intégration

| Propriété | Réponse |
|---|---|
| On peut toujours choisir n'importe quel ordre d'intégration | ❌ (valable si $f$ continue, mais les bornes doivent rester valides) |
| Il y a 6 ordres possibles pour une intégrale triple | ✅ ($3! = 6$) |
| Si les bornes de $z$ dépendent de $x$, on peut mettre $z$ à l'extérieur | ❌ (bornes non constantes → $z$ doit être à l'intérieur ou au milieu) |
| Pour choisir la variable extérieure, chercher celle avec les bornes constantes | ✅ (règle pratique) |

### Coordonnées cylindriques

| Propriété | Réponse |
|---|---|
| $dV = dr\,d\theta\,dz$ en cylindriques | ❌ (il manque le facteur $r$ : $dV = r\,dr\,d\theta\,dz$) |
| Le Jacobien en cylindriques est $r_{\max}$ | ❌ (c'est $r$, la variable d'intégration) |
| $x^2+y^2 = r^2$ en cylindriques | ✅ |
| Les cylindriques sont utiles quand le domaine a un axe de symétrie autour de l'axe $z$ | ✅ |

### Coordonnées sphériques (convention EPFL : $z = r\cos\varphi$)

| Propriété | Réponse |
|---|---|
| $dV = r^2\sin\varphi\,dr\,d\theta\,d\varphi$ | ✅ |
| $dV = r^2\,dr\,d\theta\,d\varphi$ (sans $\sin\varphi$) | ❌ (oubli du Jacobien) |
| $\varphi \in [0,\pi/2]$ correspond à $z \geq 0$ | ✅ ($\cos\varphi \geq 0$) |
| $\varphi \in [0,\pi/2]$ correspond à $z \leq 0$ | ❌ (c'est $\varphi \in [\pi/2, \pi]$) |
| $\theta \in [0,\pi]$ correspond à $y \geq 0$ | ✅ ($\sin\theta \geq 0$) |
| $\theta \in [-\pi/2, \pi/2]$ correspond à $x \geq 0$ | ✅ ($\cos\theta \geq 0$) |
| Le cône $z = \sqrt{x^2+y^2}$ correspond à $\varphi = \pi/4$ en sphériques | ✅ ($\tan\varphi = 1 \Rightarrow \varphi = \pi/4$) |
| Le cône $z = k\sqrt{x^2+y^2}$ correspond à $\varphi = \arctan(k)$ | ❌ (c'est $\varphi = \arctan(1/k)$) |
| Un cône correspond à $r$ fixe en coordonnées sphériques | ❌ (cône = $\varphi$ fixe ; sphère = $r$ fixe) |
| $x^2+y^2+z^2 = R^2$ se traduit par $r = R$ en sphériques | ✅ |

### Applications triples

| Propriété | Réponse |
|---|---|
| $\iiint_S 1\,dV = \text{Vol}(S)$ | ✅ |
| Le volume d'une boule de rayon $R$ est $\frac{4}{3}\pi R^3$ | ✅ |
| $M_{yz} = \iiint x\,\delta\,dV$ (moment par rapport au plan $yz$) | ✅ |
| $M_{yz}$ contient la variable $z$ | ❌ (contient $x$) |
| $\bar{x} = M_{yz}/M$ | ✅ |
| $\bar{z} = M_{yz}/M$ | ❌ (c'est $\bar{z} = M_{xy}/M$, où $M_{xy} = \iiint z\,\delta\,dV$) |
| Si $S$ est symétrique / plan $x=0$ et $\delta$ paire en $x$, alors $\bar{x}=0$ | ✅ |
| $\bar{f} = \iiint_S f\,dV$ (valeur moyenne en 3D) | ❌ (il faut diviser par $\text{Vol}(S)$) |
