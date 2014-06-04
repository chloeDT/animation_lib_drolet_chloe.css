# Librairie CSS3

Bonjour, vous avez dans vos mains une librairie contenant diverses animations que vous pouvez utiliser sur le web. Ce document vous permettra de comprendre comment utiliser ces animations à leur plein potentiel.

## Comment intégrer la libraire dans votre site web?

#### Étape 1

Prenez le fichier `animation_lib_drolet_chloe.css` et glissez-le dans le dossier où vous avez disposez de vos fichiers css ou à la base du dossier. 

#### Étape 2

Pour utiliser le fichier d’animation sur votre site web, vous devez relier le fichier css à votre page html. Pour se faire écrire `<link rel=“stylesheet" href=“animation_lib_drolet_chloe.css”>` entre le `<head>…</head>` de votre fichier html.



## Comment utiliser les animations sur votre site web?

#### Étape 1

Pour utiliser les animations de la libraire sur votre site vous devez simplement ajouter la classe `animation` aux objets que vous voulez animer ainsi que la classe titre de l’animation voulu.

Par exemple, vous voulez utiliser `flotter` dans un div, le code ressemblera à ça:

```html
<div class="animation flotter"></div>
```

#### Étape 2

Maintenant vous voulez augmenter le delay, la duration ou le nombre de fois que l’animation joue. Voici quoi faire:

1. Vous devez créé un id relié à votre élément à animer.

2. Ensuite, placez une ou plusieurs des propriétés choisies:

```css
#votreObjet{
/* La durée de l’animation dans un cycle */
	-webkit-animation-duration: 2s;
    	-moz-animation-duration: 2s;
	-o-animation-duration: 2s;
   	animation-duration: 2s;

/* Le délai en secondes avant que l’animation commence */

	-webkit-animation-delay: 2s;
	-moz-animation-delay: 2s;
	-o-animation-delay: 2s;
	animation-delay: 2s;

	/* Le nombre de fois que l’animation va se dérouler. Vous pouvez entre le nombre de fois exact que vous voulez que l'animation se déroule ou vous pouvez écrire infinite (infini de fois) */

	-webkit-animation-iteration-count: infinite;
    	-moz-animation-iteration-count: infinite;
   	-o-animation-iteration-count: infinite;
	animation-iteration-count: infinite;
}

```

** Si vous voulez que votre animation joue à l’infini seulement ajouter la classe `infini` à votre objet.



## 3. Qu’est-ce que font les animations exactement?

### Animation - flotter

L’animation `flotter` fait un mouvement de haut en bas (sur l’axe des Y) tout en perdant de l’opacité ainsi qu’un changement de couleur. Vous pouvez les trois propriétés sans aucun problème.

### Animation - glisse_disparait 

L’animation `glisse_disparait` glisse de gauche à droite (sur l’axe des X) tout en disparaissant (opacité devient 0) et changeant de couleur. Vous pouvez les trois propriétés sans aucun problème.

### Animation - rotation

L’animation `rotation` fait un mouvement de va et vient (sur l’axe des X) tout en faisait une rotation et changeant de couleur. Vous pouvez les deux propriétés sans aucun problème.

### Animation - coeur_battant

L’animation `coeur_battant` fait un mouvement de grossir et rapetisser pour donner l’effet d’un mouvement de coeur qui bat. L’animation comment avec une opacité de 0%, à 50% elle devient 100% d’opacité et redevient 0% d’opacité.  Vous pouvez modifier les 3 propriétés sans aucun problème.

### Animation - bondir

L’animation `bondir` fait le mouvement d’une balle qui rebondit. Elle fait un mouvement sur l’axe des Y tout en s’écrasant à l’atterrissage. Une certaine vitesse produit quand la balle saute.
