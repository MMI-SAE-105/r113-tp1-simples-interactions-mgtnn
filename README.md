- nom : Grosstephan
- prénom : Marion
- URL Netlify :

# Travail

Documentation JS/DOM : [MDN](https://developer.mozilla.org/fr/)

## Simples interactions

### Changer la couleur du texte

Faire dans la console les commandes suivantes :

![](/assets/img/changer-la-couleur-du-texte.png)

aMettreEnRouge = document.querySelector("#a-mettre-en-rouge")
<p id=​"a-mettre-en-rouge">​…​</p>​
aMettreEnRouge.style.color = "red"
'red'

### Réagir à un click
enRougeSuiteAClick = document.querySelector("#en-rouge-suite-a-click")
<button id=​"en-rouge-suite-a-click">​En rouge suite à un click​</button>​
enRougeSuiteAClick.addEventListener("click", (evt)=>{
    enRougeSuiteAClick.style.color = "red"
});
undefined

Faire dans la console les commandes suivantes :

![](/assets/img/reagir-a-un-click.png)

Testez en cliquant sur le bouton.

## Collections d'éléments

### Trouvez tous les 'H2' du document
collH2 = document.querySelectorAll("h2")
NodeList(3) [h2, h2, h2]
collH2.forEach((elm)=>{
    elm.addEventListener("click", (evt)=>{
        evt.target.style.color = "red";
    });
});

- Puis pour chacun,
  - suite à un click,
    - mettre la cible de l'événement en rouge

Faire dans la console les commandes suivantes :

![](/assets/img/collections-d-elements.png)

Testez le click sur les 'H2'.

## Script externe

Refaire les codes dans le fichier `/src/js/script.js` .

Les déclarations de variables doivent être précédées de `const` .

Recharger la page et tester le click sur le bouton et les 'H2'.

** Ne pas oublier de "Commit" et "Push" pour rendre **
