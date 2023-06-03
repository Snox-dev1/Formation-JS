
# Résumé Javascript. (ce qu'a expliquer Xavier)

## 1. Creation de variables

- les variables peuvent avoir pleins de noms
	- `let MaVariable1`
	- `let MAVARIABLE1`
	- `let mA_VaRiAbLe`
- l'important est de garder une logique dans le nommage de variables (pour retenir plus facilement)
	- Les conventions courantes sont :
		- PascalCase : la première lettre de chaque mot est en majuscule (`let MaSuperVariable`)
		-   camelCase : le premier mot en minuscule, puis chaque mot suivant en majuscule (`let maSuperVariable`)
		-   snake_case : tout en minuscule, séparé par des underscores (`let ma_super_variable`)
		-   ALL_CAPS : comme snake_case, mais tout en majuscules (`let MA_SUPER_VARIABLE`)
		-   Les variables doivent avoir des noms significatifs pour que les autres personnes puissent rapidement comprendre leur utilité :
    
    -   Exemples à éviter :
        -   `let variableSuperCool`
        -   `let jeSaisPas`
    -   Exemples recommandés :
        -   `let nombreDeVoiture`
        -   `let ageDuChatDeXavier`
-   Les variables ne peuvent pas commencer par un chiffre :
    
    -   Exemples à éviter :
        -   `let 1erNombre`
        -   `let 2emeNombre`
    -   Exemples recommandés :
        -   `let premierNombre`
        -   `let deuxiemeNombre`
-   Les variables ne peuvent pas contenir de mots réservés du langage (fonctions, boucles, conditions, etc.) :
    
    -   Exemples à éviter :
        -   `let let`
        -   `let if`
    -   Exemples recommandés :
        -   `let maVariable`
        -   `let maVariable2`

### 2. Les types

#### 2.A Les types de base

##### 2.A.1 Les nombres (Number)

Les nombres sont des nombres entiers ou décimaux.

Exemples :

```javascript
let nombre = 1;
let nombre2 = 2.5;
```

##### 2.A.2 Les chaînes de caractères (String)

Les chaînes de caractères sont des mots ou des phrases.

Exemples :

```javascript
let chaineDeCaractere = "Bonjour";
let chaineDeCaractere2 = "Je m'appelle Hubert";
```

##### 2.A.3 Les booléens (Boolean)

Les booléens sont des valeurs qui ne peuvent être que vraies ou fausses.

Exemples :

```javascript
let booleen = true;
let booleen2 = false;
```

##### 2.A.4 Les tableaux (Array)

Les tableaux sont des listes de valeurs et peuvent contenir plusieurs types de valeurs. Ils sont toujours entourés de crochets `[]`.

Exemples :

```javascript
let tableau = [1, 2, 3, 4, 5];
let tableau2 = ["Bonjour", "Je", "M'appelle", "Hubert"];
```

##### 2.A.5 Les objets (Object)

Les objets sont des listes de valeurs et peuvent contenir plusieurs types de valeurs. Ils sont toujours entourés d'accolades `{}`.

Exemple :

```javascript
let objet = {
    nom: "Hubert",
    age: 25,
    estCool: true,
    hobbies: ["Manger", "Dormir", "Coder"]
};
```

#### 2.B Les types avancés

- Les `int`, `float`, `double`, etc. sont des types de nombres.

##### 2.B.1 Les nombres entiers (Int)

Les nombres entiers sont des nombres sans décimales.

Exemple :

```javascript
let nombreEntier = 1;
```

##### 2.B.2 Les nombres décimaux (Float)

Les nombres décimaux sont des nombres avec décimales.

Exemple :

```javascript
let nombreDecimal = 1.5;
```


## 3. Les fonctions

### 3.A Reconnaître une fonction
- Les fonctions sont des blocs de code qui peuvent être appelés plusieurs fois à différents endroits du code, et sont toujours suivis de parenthèses `()`.

#### 3.A.1 Les fonctions qui permettent de récupérer un élément HTML (getElementById, getElementsByClassName, etc...)
- Ces fonctions permettent de récupérer un élément HTML (balise, id, class, etc...) et de le stocker dans une variable pour pouvoir l'utiliser plus tard.


```javascript
// getElementById permet de récupérer un élément HTML par son id (id="monElement") 
// (ne peut récupérer qu'un seul élément)
let monElement = document.getElementById("monElement"); 
```

```javascript
// getElementsByClassName permet de récupérer un élément HTML par sa classe (class="mesElements") 
// (peut récupérer plusieurs éléments) (retourne un tableau)
let mesElements = document.getElementsByClassName("mesElements"); 
```
```javascript
// getElementsByTagName permet de récupérer un élément HTML par son nom de balise 
// (peut récupérer plusieurs éléments) (retourne un tableau)
let mesElements2 = document.getElementsByTagName("p"); 
```
```javascript
// querySelector permet de récupérer un élément HTML par son id (id="monElement") 
// (ne peut récupérer qu'un seul élément)
let monElement2 = document.querySelector("#monElement"); 
```
```javascript
// querySelectorAll permet de récupérer un élément HTML par sa classe (class="mesElements") 
//(peut récupérer plusieurs éléments) (retourne un tableau)
let mesElements3 = document.querySelectorAll(".mesElements"); 
```

Comme vous pouvez le voir, ils sont précédés par une variable suivie d'un signe égal `=` et d'une fonction (`document.getElementById("monElement")`). Les parenthèses peuvent contenir des paramètres (`document.getElementById("monElement")` où le paramètre est "monElement").

Ces variables peuvent maintenant être utilisées pour modifier l'élément HTML (changer son contenu, sa couleur, etc...).

#### 3.A.2 Les fonctions qui permettent de modifier un élément HTML (innerHTML, style, etc...)
- Ces fonctions permettent de modifier un élément HTML (balise, id, class, etc...) mais ne peuvent pas être stockées dans une variable.

##### 3.A.2.a `innerHTML`
`innerHTML` permet de modifier le contenu d'un élément HTML (balise, id, class, etc...).

```javascript
// innerHTML est précédé d'un signe égal `=` (monElement.innerHTML = "Bonjour") va donner <p id="monElement">Bonjour</p>
monElement.innerHTML = "Bonjour"; 
```

##### 3.A.2.b `style`
`style` permet de modifier le style d'un élément HTML (balise, id, class, etc...).

```javascript
// style est précédé d'un point `.` (monElement.style.color = "red") va donner <p id="monElement" style="color: red;">Bonjour</p>
monElement.style.color = "red"; 
```

##### 3.A.2.c `classList`
`classList` permet de modifier les classes d'un élément HTML (balise, id, class, etc...).

###### 3.A.2.c.1 `add`
`add` permet d'ajouter une classe à un élément HTML (

balise, id, class, etc...).

```javascript
// add est une fonction et donc est suivi de parenthèses `()` (monElement.classList.add("maclass")) va donner <p id="monElement" class="maclass">Bonjour</p>
monElement.classList.add("maclass"); 
// add peut prendre plusieurs paramètres (monElement.classList.add("maclass", "maclass2", "maclass3");)
```

###### 3.A.2.c.2 `remove`
`remove` permet de supprimer une classe à un élément HTML (balise, id, class, etc...).

```javascript
// remove est une fonction et donc est suivi de parenthèses `()` (monElement.classList.remove("maclass")) va donner <p id="monElement">Bonjour</p>
monElement.classList.remove("maclass"); 
// remove peut prendre plusieurs paramètres (monElement.classList.remove("maclass", "maclass2", "maclass3");)
```

Il est également possible de donner une classe à un élément HTML (balise, id, class, etc...) et de le retrouver grâce à `getElementsByClassName` ou `querySelectorAll` (voir 3.A.1).

```javascript
monElement.classList.add("maclass");

monElement2 = document.getElementsByClassName("maclass"); // monElement2 va contenir <p id="monElement" class="maclass">Bonjour</p>
```

#### 3.A.3 Les fonctions qui permettent de créer un élément HTML (createElement, appendChild, etc...)
Ces fonctions permettent de créer un élément HTML (balise, id, class, etc...).

##### 3.A.3.a `createElement`
`createElement` permet de créer un élément HTML (balise, id, class, etc...).
`createElement` est suivi de parenthèses `()` (ici le paramètre est `p`)
```javascript

let monNouvelElement = document.createElement("p"); 
```
`createElement("p")` va donner `<p></p>` (un élément HTML vide et non affiché sur la page)

##### 3.A.3.b `appendChild`
`appendChild` permet d'ajouter un élément HTML (balise, id, class, etc...) à un autre élément HTML (balise, id, class, etc...).
`appendChild` est une fonction et donc est suivi de parenthèses `()`  (ici le paramètre est `monNouvelElement`)
```javascript

monElement.appendChild(monNouvelElement); 
```
`appendChild(monNouvelElement)` va donner `<p id="monElement">Bonjour <p></p> </p>` (`monNouvelElement` est maintenant un enfant de `monElement`)
##### 3.A.3.c `removeChild`
`removeChild` permet de supprimer un élément HTML (balise, id, class, etc...) à un autre élément HTML (balise, id, class, etc...).
`removeChild` est une fonction et donc est suivi de parenthèses `()` (ici le paramètre est `monNouvelElement`)
```javascript
 
monElement.removeChild(monNouvelElement);
```
`removeChild(monNouvelElement)` va donner `<p id="monElement">Bonjour</p>` (`monNouvelElement` n'est plus un enfant de "monElement")