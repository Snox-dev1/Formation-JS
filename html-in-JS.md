# Crée des elements html a l'aide de javascript

## Recuperer un element html

### getElementById 
`getElementById` permet de recuperer un element html a partir de son id

```javascript
let element = document.getElementById("id");
```	



### getElementsByClassName
`getElementsByClassName` permet de recuperer un element html a partir de sa classe    
    
```javascript
let elements = document.getElementsByClassName("maClasse");
```



### getElementsByTagName
`getElementsByTagName` permet de recuperer un element html a partir de son tag (p, div, h1, ...)
```javascript
let elements = document.getElementsByTagName("p");
```



### querySelector
`querySelector` permet de recuperer un element html a partir de son id, sa classe ou son tag
```javascript
let element = document.querySelector("#id");
```



### querySelectorAll
`querySelectorAll` permet de recuperer des elements html a partir leur classe ou tag
```javascript
let elements = document.querySelectorAll(".maClasse");
```



## Creer un element html

### createElement
`createElement` permet de creer un element html a partir de son tag (p, div, h1, ...)

```javascript
let element = document.createElement("p");
```
 
### appendChild
`appendChild` permet d'ajouter un element html a un autre element html

```javascript
let element = document.createElement("p");
let parent = document.getElementById("parent");
parent.appendChild(element);
```


## Modifier un element html

### innerHTML
`innerHTML` permet de modifier le contenu d'un element html

```javascript
let element = document.getElementById("element");
element.innerHTML = "nouveau contenu";
```

### style
`style` permet de modifier le style d'un element html

```javascript
let element = document.getElementById("element");
element.style.color = "red";
```

### classList
`classList` permet de modifier les classes d'un element html

#### Ajouter une class
`add()` permet d'ajouter une classe a un element html


```javascript
let element = document.getElementById("element")
element.classlist.add("maClass")
```

#### Supprimer une class
`remove()` permet de supprimer une classe a un element html

```javascript
let element = document.getElementById("element")
element.classlist.remove("maClass")
```

#### Toggle une class
`toggle()` permet d'ajouter ou de supprimer une classe a un element html

```javascript
let element = document.getElementById("element")
element.classlist.toggle("maClass")
```

#### setAttribute
`setAttribute` permet de modifier/ajouter un attribut d'un element html

```javascript
let element = document.getElementById("element")
element.setAttribute("id", "nouvelId")
```

#### removeAttribute
`removeAttribute` permet de supprimer un attribut d'un element html

```javascript
let element = document.getElementById("element")
element.removeAttribute("id")
```

#### getAttribute
`getAttribute` permet de recuperer la valeur d'un attribut d'un element html

```javascript
let element = document.getElementById("element")
let id = element.getAttribute("id")
```













