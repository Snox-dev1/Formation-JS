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

## Les conditions ternaires

La condition ternaire permet de tester une condition, si elle est vraie, la première expression est retournée, sinon, la deuxième expression est retournée.

```javascript
condition ? expression1 : expression2
```

exemple :

```javascript
const age = 18;
let majeur = age >= 18 ? true : false;
```



## Les conditions multiples

### La condition `switch`

La condition `switch` permet de tester plusieurs conditions, si une est vraie, le code entre les accolades est exécuté.

```javascript
switch (expression) {
    case valeur1:
        // code à exécuter si expression est égal à valeur1
        break;
    case valeur2:
        // code à exécuter si expression est égal à valeur2
        break;
    default:
        // code à exécuter si expression n'est égal à aucune des valeurs
}
```
### La condition `switch` combinée

La condition `switch` combinée avec `&&` permet de tester plusieurs conditions, si elles sont toutes vraies, le code entre les accolades est exécuté.

```javascript
switch (expression) {
    case valeur1 && valeur2:
        // code à exécuter si expression est égal à valeur1 et valeur2
        break;
    case valeur3 && valeur4:
        // code à exécuter si expression est égal à valeur3 et valeur4
        break;
    default:
        // code à exécuter si expression n'est égal à aucune des valeurs
}
```






