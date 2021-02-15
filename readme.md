
# Introduction

L'objectif du document est la création d'une *cheat sheet* ou "feuille de triche". 

L'ensemble des fonctions que vous devez documenter se trouvent dans ce document, à vous de  remplir les espaces vides 😉

Ce document pourra vous suivre tout au long de vos études, n'hésitez à le compléter au fur et à mesure.

---

Pour compléter le document, vous utiliserez la fonction **fork** de GitHub pour copier ce projet dans votre espace personnel.

[Si besoin, rendez-vous dans ce dépôt pour revoir les bases de Javascript](https://github.com/Maxence-Machu/javascript-basic-memo)

---

## La fonction GetElementByID()

### Que fait la fonction ?
La méthode getElementById() renvoie un objet qui représente l'élément dont la propriété  id correspond à la chaîne de caractères spécifiée.
Étant donné que les ID d'élément doivent être uniques, s'ils sont spécifiés, ils constituent un moyen utile d'accéder rapidement à un élément spécifique.

### Pourquoi l'utiliser ?
La fonction getElementById doit être utilisée si l'on veut utiliser un élément du DOM en HTML grâce à Javascript 

#### Note supplémentaire
La fonction getElementByID est à ne pas confondre avec la fonction *getElementsByClassName*. 
Les ID dans une page web sont uniques, on ne peut donc pas récupérer plusieurs éléments avec cette fonction. 

### Exemple de code:
```javascript
let element = document.getElementByID('mon-element');
console.log(element);
```

## La fonction GetElementsByClassName()

### Que fait la fonction ?
La méthode GetElementsByClassName retourne une collection HTML  contenant une référence sur tous les éléments ayant les noms de classes passés en paramètre. Quand la méthode est appelée sur l'objet document, la recherche s'effectue dans le document complet, noeud racine compris.

### Pourquoi l'utiliser ?
...

### Exemple de code:
```javascript
// CODE ```
element.getElementsByClassName('test');
```


## La fonction querySelector() et querySelectorAll()

### Que fait la fonction ?
La méthode querySelector (et querySelectorALL) de l'interface Document retourne le premier Element  dans le document correspondant au sélecteur - ou groupe de sélecteurs - spécifié(s), ou `null` si aucune correspondance n'est trouvée.

### Pourquoi l'utiliser ?
...

### Exemple de code:
```javascript
// CODE```
var el = document.querySelector(".maclasse");

```

## La fonction addEventListener()

### Que fait la fonction ?
La méthode addEventListener d'EvenTarget  installe une fonction à appeler chaque fois que l'événement spécifié est envoyé à la cible. Les cibles courantes sont un Element, le Document lui-même et une Window, mais elle peut être tout objet prenant en charge les évènements comme `[XMLHttpRequest]

### Pourquoi l'utiliser ?
"addEventListener" fonctionne en ajoutant une fonction, ou un objet implémentant EventListener, à la liste des écouteurs d'évènements du type d'évènement spécifié dans la EventTarget dans laquelle il est appelé.

### Exemple de code:
```javascript
// CODE ```
// Fonction pour changer le contenu de t2
function modifierTexte() {
  var t2 = document.getElementById("t2");
  if (t2.firstChild.nodeValue == "trois") {
    t2.firstChild.nodeValue = "deux";
  } else {
    t2.firstChild.nodeValue = "trois";
  }
}

// Ajouter un écouteur d'évènements à la table
var el = document.getElementById("aLExterieur");
el.addEventListener("click", modifierTexte, false);

```

## La fonction stopPropagation()

### Que fait la fonction ?
Évite que l'évènement courant ne se propage plus loin dans les phases de capture et de déploiement.

### Pourquoi l'utiliser ?
Pour éviter que...

### Exemple de code:
```javascript
// CODE
```

## La fonction addEventListener('mousemove', maFonction)

### Que fait la fonction ?
L'évènement `mousemove` est déclenché à partir d'un élément lorsqu'un dispositif de pointage (ex. une souris) est déplacé lorsque le curseur est à l'intérieur de l'élément.

### Pourquoi l'utiliser ?
...

### Exemple de code:
```javascript
// CODE```
// Un booléen qui, lorsqu'il est vrai, indique que le déplacement de
// la souris entraîne un dessin sur le canevas
let isDrawing = false;
let x = 0;
let y = 0;

const myPics = document.getElementById('myPics');
const context = myPics.getContext('2d');

// On récupère le décalage du canevas en x et y par rapport aux bords
// de la page
const rect = myPics.getBoundingClientRect();

// On ajoute les gestionnaires d'évènements pour mousedown, mousemove
// et mouseup
myPics.addEventListener('mousedown', e => {
  x = e.clientX - rect.left;
  y = e.clientY - rect.top;
  isDrawing = true;
});

myPics.addEventListener('mousemove', e => {
  if (isDrawing === true) {
    drawLine(context, x, y, e.clientX - rect.left, e.clientY - rect.top);
    x = e.clientX - rect.left;
    y = e.clientY - rect.top;
  }
});

window.addEventListener('mouseup', e => {
  if (isDrawing === true) {
    drawLine(context, x, y, e.clientX - rect.left, e.clientY - rect.top);
    x = 0;
    y = 0;
    isDrawing = false;
  }
});

function drawLine(context, x1, y1, x2, y2) {
  context.beginPath();
  context.strokeStyle = 'black';
  context.lineWidth = 1;
  context.moveTo(x1, y1);
  context.lineTo(x2, y2);
  context.stroke();
  context.closePath();
}
```

## La fonction parseInt()

### Que fait la fonction ?
...

### Pourquoi l'utiliser ?
...

### Exemple de code:
```javascript
// CODE
```


## La variable "event" dans le code suivant:

### Code:
```javascript
element.addEventListener('event-name', function(event) {
  console.log(event);
});
```

### Qu'est-ce que cette variable ?
...

### Pourquoi l'utiliser ?
...


