# Les fonctions
## Définition

Une fonction est un bloc de code qui peut être appelé plusieurs fois dans un programme. Elle peut prendre des paramètres et retourner une valeur ou non.

Votre fonction peut avoir un nom, comme pour les variables, il doit commencer par une lettre ou un underscore, et ne peut contenir que des lettres, des chiffres et des underscores.

```javascript
function calcul() {
    console.log("Je suis un calcul");
}
```

## Appel

Pour appeler une fonction, il suffit d'écrire son nom suivi de parenthèses.

```javascript
nomDeMaFonction(); // dans la console: Je suis un calcul
```

## Return

Une fonction peut retourner une valeur, pour cela, il faut utiliser le mot clé `return`. Une fois que la fonction a rencontré un `return`, elle s'arrête et retourne la valeur. Si vous avez plusieurs `return` dans votre fonction, seule la première valeur sera retournée.

```javascript
function calcul() {
    return "je suis un calcul";
}

console.log(calcul()); // dans la console: je suis un calcul
```

Si vous ne mettez pas de `return` dans votre fonction, elle retournera `undefined`.

```javascript
function calcul() {
    console.log("je suis un calcul"); // dans la console: je suis un calcul
}

console.log(calcul()); // dans la console: je suis un calcul, undefined
```


## Arguments

Une fonction peut prendre des paramètres, pour cela, il faut les déclarer entre les parenthèses. Ces paramètres sont des variables locales à la fonction, ils ne sont pas accessibles en dehors de la fonction.

### Types d'arguments
Vous pouvez utiliser n'importe quel type de variable comme argument d'une fonction.

- chaîne de caractères (string) : `"je suis une chaîne de caractères"`
- nombre (number) : `1`
- valeur booléenne (boolean) : `true`
- variable (variable) : `maVariable`


#### Exemple :


```javascript
function calcul(nb1, nb2, operateur) {
    const result = nb1 +operateur+ nb2;
    return result
}

console.log(calcul(1, 2, "+")); // dans la console: undefined
```


sachant que l'operateur est un string et que les deux nombres sont des nombres. il faut une condition pour chaque opérateur. (voir conditions.md)

```javascript

function calcul(nb1, nb2, operateur) {
    if (operateur === "+") {
        const result = nb1 + nb2;
        return result;
    } else if (operateur === "-") {
        return nb1 - nb2;
    } else if (operateur === "*") {
        const result = nb1 * nb2;
        return result;
    } else if (operateur === "/") {
        return nb1 / nb2;
    } else {
        return "erreur";
    }
}

console.log(calcul(1, 2, "+")); // dans la console: 3
console.log(calcul(1, 2, "-")); // dans la console: -1
console.log(calcul(1, 2, "*")); // dans la console: 2
console.log(calcul(1, 2, "/")); // dans la console: 0.5
console.log(calcul(1, 2, "a")); // dans la console: erreur

// ou

const result1 = calcul(1, 2, "+");
console.log(result1); // dans la console: 3
```

La fonction `calcul` prend deux arguments, `arg1` et `arg2`, et retourne la somme de ces deux arguments.


## les différents types de fonctions 

### Fonctions déclarées

Une fonction déclarée est une fonction qui est déclarée avec le mot clé `function`. Elle peut être appelée avant sa déclaration.

```javascript
maFonction(); // dans la console: je suis une fonction

function maFonction() {
    console.log("je suis une fonction");
}
```

### Fonctions anonymes

Une fonction anonyme est une fonction qui n'a pas de nom. Elle peut être stockée dans une variable ou être utilisée comme argument d'une autre fonction.

```javascript
const maFonction = function() {
    console.log("je suis une fonction");
}

maFonction(); // dans la console: je suis une fonction
```

### Fonctions fléchées

Une fonction fléchée est une fonction qui n'a pas de nom. Elle peut être stockée dans une variable ou être utilisée comme argument d'une autre fonction.

```javascript
const maFonction = () => {
    console.log("je suis une fonction");
}

maFonction(); // dans la console: je suis une fonction
```

### Fonctions auto-exécutées

Une fonction auto-exécutée est une fonction qui s'exécute automatiquement. Elle est déclarée dans une parenthèse, et est suivie d'une autre paire de parenthèses qui contient les arguments de la fonction.

```javascript
(function() {
    console.log("je suis une fonction");
})(); // dans la console: je suis une fonction
```
