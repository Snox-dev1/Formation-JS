# Les Tableaux en JavaScript

Les tableaux sont des structures de données utilisées pour stocker des collections de valeurs dans JavaScript. Ils permettent de regrouper des éléments connexes et de les manipuler de manière efficace. Dans ce tutoriel, nous allons apprendre comment déclarer et utiliser des tableaux en JavaScript.

## Déclaration de tableaux

Pour déclarer un tableau en JavaScript, vous pouvez utiliser la syntaxe suivante :

```javascript
let fruits = ['pomme', 'banane', 'orange'];
```

Dans cet exemple, nous avons déclaré un tableau appelé `fruits` qui contient trois éléments : `'pomme'`, `'banane'` et `'orange'`.

## Accéder aux éléments d'un tableau

Pour accéder aux éléments d'un tableau, vous pouvez utiliser l'indice de l'élément. Les indices commencent à zéro pour le premier élément et augmentent de un pour chaque élément suivant.

```javascript
let fruits = ['pomme', 'banane', 'orange'];

console.log(fruits[0]);  // Affiche 'pomme'
console.log(fruits[1]);  // Affiche 'banane'
console.log(fruits[2]);  // Affiche 'orange'
```

## Modifier les éléments d'un tableau

Vous pouvez modifier les éléments d'un tableau en utilisant l'indice de l'élément et l'opérateur d'assignation (=).

```javascript
let fruits = ['pomme', 'banane', 'orange'];

fruits[1] = 'kiwi';
console.log(fruits);  // Affiche ['pomme', 'kiwi', 'orange']
```

Dans cet exemple, nous avons modifié l'élément à l'indice 1 du tableau `fruits` et l'avons remplacé par `'kiwi'`.

## Ajouter et supprimer des éléments d'un tableau

JavaScript fournit plusieurs méthodes pour ajouter et supprimer des éléments d'un tableau. En voici quelques-unes :

### Ajouter des éléments :

- `push`: ajoute un ou plusieurs éléments à la fin du tableau.
```javascript
let fruits = ['pomme', 'banane'];

fruits.push('orange');
console.log(fruits);  // Affiche ['pomme', 'banane', 'orange']
```

- `unshift`: ajoute un ou plusieurs éléments au début du tableau.
```javascript
let fruits = ['pomme', 'banane'];

fruits.unshift('orange');
console.log(fruits);  // Affiche ['orange', 'pomme', 'banane']
```

### Supprimer des éléments :

- `pop`: supprime le dernier élément du tableau et renvoie cet élément.
```javascript
let fruits = ['pomme', 'banane', 'orange'];

let dernierFruit = fruits.pop();
console.log(fruits);        // Affiche ['pomme', 'banane']
console.log(dernierFruit);  // Affiche 'orange'
```

- `shift`: supprime le premier élément du tableau et renvoie cet élément.
```javascript
let fruits = ['pomme', 'banane', 'orange'];

let premierFruit = fruits.shift();
console.log(fruits);      // Affiche ['banane', 'orange']
console.log(premierFruit); // Affiche 'pomme'
```
