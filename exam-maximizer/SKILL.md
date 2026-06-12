---
name: exam-maximizer
description: >
  Use this skill IMMEDIATELY whenever the user asks "comment apprendre [sujet] pour l'examen",
  "comment réviser [sujet]", "comment maîtriser [sujet] pour l'exam", or sends a photo of a
  notion théorique avec une question sur comment l'aborder à l'examen. Le skill cherche dans
  les séries et examens passés du cours d'Analyse 2 (MATH-106 EPFL) pour analyser COMMENT
  cette notion apparaît concrètement dans les exercices, puis produit un guide ciblé
  "maximisation examen" sauvegardé dans maximisation_examen.md. Toujours utiliser ce skill
  même si le sujet semble simple — l'analyse des patterns d'examen est toujours utile.
---

# Skill : Maximisation Examen — Analyse 2

## Objectif

Quand l'utilisateur demande comment apprendre/réviser une notion pour l'examen, tu dois :
1. Identifier la notion (depuis le message ou la photo)
2. Chercher comment elle apparaît dans les séries et examens passés
3. Produire un guide ciblé et pragmatique
4. Sauvegarder dans `maximisation_examen.md`

---

## Étape 1 — Identifier la notion

Extrais le sujet depuis :
- Le texte du message ("comment apprendre les séries de Taylor")
- Une photo de cours (lis le contenu de l'image)
- Le contexte de la conversation

Si le sujet est flou, demande une clarification courte avant de continuer.

---

## Étape 2 — Chercher dans les séries

Les séries se trouvent dans :
- `/Users/liamvancamp/Desktop/EPFL/BA2/analyse_2/séries/` → Série_01.pdf à Série_14.pdf + Solution_01.pdf à Solution_14.pdf

**Méthode :**
- Référence-toi au plan S1-S14 dans `_formules/PLAN_ANALYSE_S1-S14.md` pour cibler les bonnes séries
- Lis les PDFs des séries pertinentes pour identifier les exercices sur la notion
- Note : type d'exercice (calcul direct, preuve, vrai/faux, IVP), niveau de difficulté, pièges récurrents
- Lis aussi les solutions pour comprendre la démarche attendue

---

## Étape 3 — Chercher dans les examens passés

Les examens se trouvent dans :
- `/Users/liamvancamp/Desktop/EPFL/BA2/analyse_2/examens/`

Si le dossier est vide, note-le et base-toi sur les séries + patterns typiques EPFL.

---

## Étape 4 — Produire le guide

Structure le guide ainsi :

```
# Comment maîtriser [NOTION] pour l'examen

## Ce qui est testé à l'examen
- Type d'exercice (calcul, preuve, vrai/faux, IVP...)
- Niveau de difficulté typique
- Apparition dans les séries : S__, Ex.__

## Ce qu'il faut savoir par cœur
- Définitions clés
- Formules à mémoriser
- Conditions / cas limites

## Marche à suivre (comment attaquer à l'examen)
1. ...
2. ...

## Pièges classiques
- ...

## Exercices à refaire en priorité
- Série __, Ex. __ (pourquoi : ...)

## Liens avec d'autres notions
- ...
```

---

## Étape 5 — Sauvegarder

Ajoute le guide dans :
`/Users/liamvancamp/Desktop/EPFL/BA2/analyse_2/théorie/maximisation_examen.md`

Si le fichier existe déjà, **ajoute** la nouvelle section à la fin avec un séparateur `---`.

---

## Règles

- Cite les numéros de séries/exercices réels trouvés dans les PDFs
- Sois pragmatique : l'objectif est de savoir quoi faire à l'examen
- Hiérarchise par fréquence d'apparition
- Après sauvegarde, présente le fichier avec `mcp__cowork__present_files`
