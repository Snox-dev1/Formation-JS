
# Les boucles en JavaScript

En JavaScript, les boucles permettent d'exécuter un bloc de code plusieurs fois. Elles sont très utiles pour automatiser des tâches répétitives ou pour parcourir des collections de données.

Il existe principalement trois types de boucles en JavaScript : la boucle `for`, la boucle `while` et la boucle `do...while`. Chacune a ses particularités et est adaptée à différentes situations.

## La boucle `for`

La boucle `for` est couramment utilisée lorsque vous connaissez à l'avance le nombre d'itérations à effectuer. Voici la syntaxe générale d'une boucle `for` :

```javascript
for (initialisation; condition; incrémentation) {
  // Bloc de code à exécuter à chaque itération
}
```

- L'initialisation est une expression ou une déclaration qui est exécutée une seule fois avant le début de la boucle.
- La condition est une expression booléenne qui est évaluée avant chaque itération. Si elle est vraie, le bloc de code est exécuté ; sinon, la boucle se termine.
- L'incrémentation est une expression exécutée après chaque itération.

Voici un exemple concret :

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

Dans cet exemple, la boucle `for` s'exécute cinq fois et affiche les nombres de 0 à 4 dans la console.

## La boucle `while`

La boucle `while` est utilisée lorsque vous ne connaissez pas à l'avance le nombre d'itérations nécessaires. Voici sa syntaxe :

```javascript
while (condition) {
  // Bloc de code à exécuter tant que la condition est vraie
}
```

- La condition est évaluée avant chaque itération. Si elle est vraie, le bloc de code est exécuté ; sinon, la boucle se termine.

Voici un exemple :

```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

Ce code produit le même résultat que l'exemple précédent avec la boucle `for`.

## La boucle `do...while`

La boucle `do...while` est similaire à la boucle `while`, mais elle garantit que le bloc de code est exécuté au moins une fois, même si la condition initiale est fausse. Voici sa syntaxe :

```javascript
do {
  // Bloc de code à exécuter
} while (condition);
```

- Le bloc de code est exécuté une fois, puis la condition est évaluée. Si elle est vraie, la boucle continue ; sinon, la boucle se termine.

Voici un exemple :

```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

Encore une fois, le résultat sera le même.
