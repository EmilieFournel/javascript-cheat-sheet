
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
...

### Pourquoi l'utiliser ?
...

### Exemple de code:
```javascript
// CODE
```

## La fonction stopPropagation()

### Que fait la fonction ?
...

### Pourquoi l'utiliser ?
...

### Exemple de code:
```javascript
// CODE
```

## La fonction addEventListener('mousemove', maFonction)

### Que fait la fonction ?
...

### Pourquoi l'utiliser ?
...

### Exemple de code:
```javascript
// CODE
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


