# Les Variables en JavaScript

Les variables sont des conteneurs utilisés pour stocker des valeurs en JavaScript. Elles permettent de manipuler et de travailler avec des données de différentes manières. Dans ce tutoriel, nous allons apprendre comment déclarer et utiliser des variables en JavaScript.

## Déclaration de variables

En JavaScript, il existe deux façons de déclarer des variables : `let` et `const`. La différence entre ces deux mots-clés réside dans la portée et la mutabilité des variables.


### `let`

La déclaration de variables avec `let` permet de créer une variable dont la portée est limitée à son bloc de code ({ }). Une variable déclarée avec `let` peut être réaffectée avec une nouvelle valeur.

```javascript
let name = "John";
```

### `const`

La déclaration de variables avec `const` est similaire à `let`, à la différence près que la valeur d'une variable déclarée avec `const` ne peut pas être modifiée une fois qu'elle est assignée. Une variable `const` doit être initialisée dès sa déclaration.

```javascript
const pi = 3.14;
```

## Utilisation des variables

Une fois que vous avez déclaré une variable, vous pouvez l'utiliser pour stocker et récupérer des valeurs. Voici comment vous pouvez utiliser des variables en JavaScript :

### Affectation de valeurs

Pour assigner une valeur à une variable, utilisez l'opérateur d'assignation (=).

```javascript
const age = 25;
const name = "John";
```

### Récupération de valeurs

Pour récupérer la valeur d'une variable, vous pouvez simplement utiliser le nom de la variable.

```javascript
console.log(age);  // Affiche 25
console.log(name); // Affiche "John"
```

### Manipulation de variables

Vous pouvez manipuler les variables en effectuant des opérations mathématiques ou en les combinant avec d'autres valeurs.

```javascript
let x = 10;
let y = 5;

const sum = x + y;        // Addition
const difference = x - y; // Soustraction
const product = x * y;    // Multiplication
const quotient = x / y;   // Division

const message = "La somme de " + x + " et " + y + " est " + sum;
console.log(message);  // Affiche "La somme de 10 et 5 est 15"
```
