# Les conditions

les conditions permettent de faire des tests sur des variables ou des valeurs. 

## Les opérateurs de comparaison 

### Les opérateurs de comparaison simples

- `==` : égal à
- `!=` : différent de
- `>` : supérieur à
- `<` : inférieur à
- `>=` : supérieur ou égal à
- `<=` : inférieur ou égal à 
- `===` : strictement égal à 
- `!==` : strictement différent de
- 
### Les opérateurs de comparaison combinés

- `&&` : ET
- `||` : OU
- `!` : NON

## Les conditions simples

### La condition `if`

La condition `if` permet de tester une condition, si elle est vraie, le code entre les accolades est exécuté.

```javascript
if (condition) {
    // code à exécuter si la condition est vraie
}
```

### La condition `if...else`

La condition `if...else` permet de tester une condition, si elle est vraie, le code entre les accolades après le `if` est exécuté, sinon, le code entre les accolades après le `else` est exécuté.

```javascript
if (condition) {
    // code à exécuter si la condition est vraie
} else {
    // code à exécuter si la condition est fausse
}
```

### La condition `if...else if...else`

La condition `if...else if...else` permet de tester plusieurs conditions, si la première est vraie, le code entre les accolades après le `if` est exécuté, sinon, si la deuxième est vraie, le code entre les accolades après le `else if` est exécuté, sinon, le code entre les accolades après le `else` est exécuté.

```javascript
if (condition1) {
    // code à exécuter si la condition1 est vraie
} else if (condition2) {
    // code à exécuter si la condition2 est vraie
} else {
    // code à exécuter si la condition1 et la condition2 sont fausses
}
```

## Les conditions combinées

### La condition `if` combinée avec `&&`

La condition `if` combinée avec `&&` permet de tester plusieurs conditions, si elles sont toutes vraies, le code entre les accolades est exécuté.

```javascript
if (condition1 && condition2) {
    // code à exécuter si la condition1 et la condition2 sont vraies
}
```

### La condition `if` combinée avec `||`

La condition `if` combinée avec `||` permet de tester plusieurs conditions, si au moins une est vraie, le code entre les accolades est exécuté.

```javascript
if (condition1 || condition2) {
    // code à exécuter si la condition1 ou la condition2 est vraie
}
```

### La condition `if` combinée avec `!`

La condition `if` combinée avec `!` permet de tester une condition, si elle est fausse, le code entre les accolades est exécuté.

```javascript
if (!condition) {
    // code à exécuter si la condition est fausse
}
```

# Les boucles

Les boucles permettent de répéter une action plusieurs fois.

## La boucle `while`

La boucle `while` permet de répéter une action tant qu'une condition est vraie.

```javascript
while (condition) {
    // code à exécuter tant que la condition est vraie
}
```
## La boucle `for`

La boucle `for` permet de répéter une action un nombre de fois défini.

```javascript
for (initialisation; condition; incrémentation) {
    // code à exécuter tant que la condition est vraie
}

// exemple

for (let i = 0; i < 10; i++) {
    console.log(i);
}
```

## La boucle `for...in`

La boucle `for...in` est une structure de contrôle en JavaScript qui permet d'itérer sur les propriétés d'un objet. Elle est particulièrement utile lorsque vous souhaitez parcourir les clés ou les propriétés d'un objet.

La syntaxe de la boucle `for...in` est la suivante :

```javascript
for (variable in objet) {
  // Instructions à exécuter pour chaque propriété
}
```
- La variable est une variable temporaire qui sera utilisée pour stocker la clé de chaque propriété à chaque itération de la boucle.
- L'objet est l'objet sur lequel vous souhaitez itérer.

Voici un exemple concret pour illustrer son utilisation :

```javascript
const voiture = {
  marque: 'Toyota',
  modèle: 'Camry',
  année: 2020
};

for (let propriete in voiture) {
  console.log(propriete + ': ' + voiture[propriete]);
}
```

Dans cet exemple, nous avons un objet voiture avec différentes propriétés telles que marque, modèle et année. La boucle `for...in` parcourt chaque propriété de l'objet et la stocke dans la variable propriete. Ensuite, nous utilisons cette variable pour accéder à la valeur de chaque propriété à l'aide de la notation entre crochets (`voiture[propriete]`) et affichons la clé et la valeur correspondantes à chaque itération

La sortie de cet exemple serait :

```
marque: Toyota
modèle: Camry
année: 2020
```




