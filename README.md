# product-presentation

## Les bases de HTML/CSS

Lien vers les bases : https://bit.ly/3jClQY8

## Déscription générale
Cette initiation permet de présenter une idée d’application web.

Ex: https://joz84.github.io/product.github.io/ .

Elle contient 6 sections :
* Une barre de navigation
* Une bannière
* Un section de présentation
* Une section présentant la bande annonce du film
* Une section présentant le casting
* Un pied de page

## Structure
Le cours est structuré de la manière suivante:
* Un fichier index.html
* Un fichier style.css avec le style À NE PAS MODIFIER
* Un fichier custom.css regroupant les propriétés modifiable
* Un dossier « images » contenant toutes les images au format jpg sauf le logo au format png ( correspondant au format produit par freelogodesign.org )

## Import de l'initiation
Lien vers le projet Github: https://github.com/ClaudineP435433/product.github.io

<img src="/images-readme/setup.png" width=700>

Cliquer sur "Clone or Download" puis sur "Download ZIP »
Décompresser le fichier sur sa machine et l’ouvrir dans sublime text

## Personnaliser le texte
### Le contenu
L’ensemble du texte à modifier est dans le fichier index.html. Avec la configuration de base de sublime text ( theme: Monokai ) le texte modifiable a la couleur syntaxique BLANCHE. Il est déconseillé de toucher le reste, car cela risque de casser la structure globale du site.

### La police
Pour personnaliser la police il faut tout d’abord choisir une police sur https://fonts.google.com.

Une fois la police choisie il faut cliquer sur le « + » en haut à droite de la fiche de la police choisie :

<img src="/images-readme/googlefonts1.png" width=700>

Un cadre Noir apparait en bas de la fenêtre. Il contient les instructions nécessaires pour importer la police dans son projet :

<img src="/images-readme/googlefonts2.png" width=700>

Dans index.html
Remplacer la ligne 9 :
```html
<!-- ########## -->
<!-- Récupérer cette ligne de code sur Google fonts : https://fonts.google.com/ -->
<link href="https://fonts.googleapis.com/css?family=Abril+Fatface" rel="stylesheet">
<!-- ########## -->
```
Dans custom.css

Modifier la ligne 3 pour changer la police des titres

Modifier la ligne 4 pour changer la police du texte
```css
/*Les polices*/
/*Récupérer cette propriété sur Google fonts : https://fonts.google.com/*/
h1, h2, h3, h4, h5, h6, i { font-family: 'Abril Fatface', cursive; }
p { font-family: 'arial'; }
```

## Personnaliser la couleur
### La couleur des titres et des cadres
Pour modifier la couleur des titres et des cadres, il faut modifier le fichier custom.css. Plus précisément, il faut modifier le code hexadécimal de la couleur dominante ( ex: #00898E ) aux ligne 7 et 8 :
```css
/*La couleur dominante*/
.circle, .navbar, .frame { border-color: #00898E; }
h1, h2, h3, h4, h5, h6, i, .item { color: #00898E; }
```

### Le fond de couleur ( dégradé ) de la présentation du Figma
Pour modifier la fond couleur, il faut encore une fois modifier le fichier custom.css. Plus précisément, les lignes 14, 15 et 16 qui sont issues de https://www.uigradients.com

<img src="/images-readme/uigradients1.png" width=700>

Cliquer sur « <> » ( Get css ) en haut à droite.

<img src="/images-readme/uigradients2.png" width=700>

Cliquer sur « CLICK TO COPY » et coller le code à la place des lignes 14, 15 et 16 du fichier custom.css :

```css
/*Le fond de couleur*/
/*Récupérer ces propriétés sur Ui Gradients: https://uigradients.com*/
.bg-color {
  background: #74ebd5;
  background: -webkit-linear-gradient(to right, #ACB6E5, #74ebd5);
  background: linear-gradient(to right, #ACB6E5, #74ebd5);
}
```

## Personnaliser les images
Il est fortement conseillé de ne pas modifier le code pour changer les images. Il est conseillé de changer les images dans le dossier images. Pour que cela fonctionne il faut que les images et le MÊME NOM et la MÊME EXTENTION. Les extensions sont toutes jpg SAUF le logo qui est en png ( car cela correspond au format fourni par freelogodesign.org ).

## Inclure une vidéo Youtube
* Aller sur Youtube et choisir une video (https://www.youtube.com/watch?v=fBuSNu2m3XA&feature=youtu.be)
* Taper clique droit sur la vidéo.
* Cliquer sur "< > Copier le code d'intégration".
<kbd>
  <img src="images-readme/youtube.png" alt="youtube">
</kbd>

* Coller le code dans le fichier html la où vous souhaitez intégrer la vidéo :

Remarque : Il est possible de changer la taille de la vidéo grâce aux attributs "width" et "height".

```html
<h3>La recette en vidéo</h3>
<iframe width="500" height="300" src="https://www.youtube.com/embed/fBuSNu2m3XA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

## Personnaliser le casting du film
Si le casting n’est pas constituée de 4 personnes il est possible d’ajouter/supprimer une fiche de présentation d’un membre dans la rubrique « Casting ». Pour cela il suffit de copier/supprimer le section comprise entre la ligne 141 et 151 du fichier index.html :
```html
<!-- ########## -->
<!-- Supprimer( ou copier-coller) ces lignes code pour supprimer (ou ajouter) un membre à la team -->
<div class="col-lg-3">
  <div class="card">
    <img src="images/team4.jpg" class="card-img-top" alt="name4">
    <div class="card-body">
      <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    </div>
  </div>
</div>
<!-- ########## -->
```

## Mise en production

La mise en production se fera sur https://github.com.

### Copier le dossier sur son compte Github

Après être retourné sur le dossier :

https://github.com/Joz84/product.github.io

<img src="/images-readme/fork1.png" width=700>

Cliquer sur « Fork » en haut à droite.

<img src="/images-readme/fork2.png" width=700>

Sélectionner votre nom.

<img src="/images-readme/fork3.png" width=700>

Le dossier est alors copier sur votre compte Github en ligne.

### Modifier et personnaliser le template

Cliquer sur le fichier que vous souhaitez modifier, par exemple: index.html :

<img src="/images-readme/custom1.png" width=700>

Puis sur le petit stylet ( « Edit this file ») en haut à droite.

<img src="/images-readme/custom2.png" width=700>

Le fichier est alors en  mode édition et modifiable.

<img src="/images-readme/custom3.png" width=700>

Copier coller le contenu de votre index.html à la place de celui-ci puis cliquer sur le bouton vert « Commit changes » en bas à gauche.

<img src="/images-readme/custom4.png" width=700>

Faite de même pour tous les fichiers/dossiers que vous souhaitez modifier.

### Mettre en ligne

Pour mettre le projet en ligne cliquer sur « Settings » en haut à droite

<img src="/images-readme/prod1.png" width=700>

Scroller jusqu’à la section « GitHub Pages »

<img src="/images-readme/prod2.png" width=700>

Cliquer sur « None » dans la rubrique « Source », puis sur « Master branch »

<img src="/images-readme/prod3.png" width=700>

Le site est alors en ligne. Un bandeau bleu avec le message « Your site is ready to be published at https://joz84.github.io/product.github.io/. »

<img src="/images-readme/prod4.png" width=700>

Rafraîchissez la page.

Au bout d’une minute, lorsque le bandeau devient vert avec le message suivant : « 
 Your site is published at https://joz84.github.io/product.github.io/ »
Le site est en ligne à l’adresse indiquée.

<img src="/images-readme/prod5.png" width=700>

Bravo votre site est en ligne!!!
