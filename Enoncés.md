# Exercices en C — Boucles et Suites (Débutant)

## Consignes générales
- Interdiction d’utiliser des fonctions
- Interdiction d’utiliser des tableaux (sauf une chaîne simple pour l’exercice 10)
- Utiliser uniquement : variables, `if`, `for`, `while`
- Langage C standard

---

## Exercice 1 — Somme des N premiers entiers
Écrire un programme qui lit un entier `N` et calcule :
S = 1 + 2 + 3 + ... + N

---

## Exercice 2 — Produit des N premiers nombres impairs
Écrire un programme qui lit un entier `N` et calcule :
P = 1 × 3 × 5 × ... (N termes)

---

## Exercice 3 — Factorielle
Écrire un programme qui lit un entier `N` et calcule :
N! = 1 × 2 × 3 × ... × N

---

## Exercice 4 — Suite de Fibonacci
Écrire un programme qui lit un entier `N` et affiche les `N` premiers termes de la suite :
0 1 1 2 3 5 8 ...

---

## Exercice 5 — Somme harmonique
Écrire un programme qui lit un entier `N` et calcule :
H = 1 + 1/2 + 1/3 + ... + 1/N  
Le résultat doit être affiché en décimal.

---

## Exercice 6 — Suite définie par récurrence
On définit la suite :
u0 = 2  
u(n+1) = 3u(n) + 1  

Écrire un programme qui lit `N` et affiche les valeurs de `u0` à `uN`.

---

## Exercice 7 — Somme des carrés
Écrire un programme qui lit un entier `N` et calcule :
S = 1² + 2² + 3² + ... + N²

---

## Exercice 8 — Calcul de puissance
Écrire un programme qui lit deux entiers `a` et `n` et calcule :
aⁿ  
Interdiction d’utiliser `pow`.

---

## Exercice 9 — Suite de Syracuse (Collatz)
Écrire un programme qui lit un entier `N` strictement positif.

Tant que `N ≠ 1` :
- si `N` est pair → `N = N / 2`
- sinon → `N = 3N + 1`

Afficher tous les termes et le nombre d’étapes.

---

## Exercice 10 — Chaîne de caractères
Écrire un programme qui lit une phrase et :
1. affiche la phrase sans les voyelles
2. affiche le nombre de caractères restants
