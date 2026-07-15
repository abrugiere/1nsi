# Numérique et Sciences Informatiques Première



## Implémentation

- Une liste est caractérisée par un ensemble de cellules.
- Chaque cellule contient donc une valeur et un lien vers la cellule suivante.
- Une liste peut être vide (la liste vide est souvent notée `None`)

## Interface
Les opérations généralement disponibles pour une liste chaînée sont :
- Créer une liste vide
- Savoir si la liste est vide
- Insérer un élément en tête de liste
- Récupérer l'élément en tête de liste

## Comparatif Tableaux / Listes chaînées

En python, le type `list` est en réalité ce que l'on appelle en algorithmique un **tableau**, c'est à dire une suite d'éléments contigus et ordonnés en mémoire. Ces éléments sont stockés en mémoire les uns à la suite des autres.

*Dans un tableau :*  

- Le temps d'accès à n'importe quel élément est rapide. Ce temps d'accès est constant quelque soit l'élément.
- L'insertion d'un élément au début ou au milieu de la liste est lente : cela oblige à décaler tous les éléments à droite de celui-ci. Le temps pris par l'insertion est proportionnel au nombre d'éléments à déplacer.


*Dans une liste chaînée :*  
- Le temps d'accès à n'importe quel élément peut être lent (proportionnel à la position de l'élément dans la liste).  
- L'insertion d'un élément à l'intérieur de la liste est rapide : il y a simplement à modifier la valeur du lien de la cellule à gauche de l'endroit d'insertion. Toutefois, avant d'arriver à l'endroit d'insertion, il faut avoir parcouru toutes les cellules précédentes ! Le temps total d'insertion est donc lui aussi linéaire.

:::danger
Nous nous servirons parfois du type `list` de Python dans la suite de ce cours, mais il ne faut pas oublier qu'il n'est pas un «vrai» type représentant une liste chaînée mais plutôt un **tableau**.
::: 

:::info
### 📝 EXERCICE 1 - Manipulation d'une liste chaînée
:::

