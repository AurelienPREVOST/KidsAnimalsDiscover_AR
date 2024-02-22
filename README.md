# Réalité augmentée avec AR.js

Cette application de réalité augmentée utilise la bibliothèque AR.js (Augmented Reality JavaScript). La documentation complète est disponible [ici](https://ar-js-org.github.io/AR.js-Docs/).

## Utilisation

L'application utilise une partie spécifique de la librairie AR.js. Dans le dossier `printableFiles`, vous trouverez des lettres imprimables ou exposables sur une tablette ou un smartphone directement à la caméra du navigateur qui exécutera l'application.

En explorant le code, quelques points clés à noter :

- Chaque modèle 3D est entouré d'une balise "a-marker".
- Cette balise HTML appartient à la librairie AR.js et a un type spécifié. Dans ce cas, nous utilisons 'pattern' car nous travaillons avec des détecteurs de type patt. Consultez la documentation pour en savoir plus.

## Création de modèles de détection

Pour créer des patterns de détection, vous pouvez utiliser l'outil disponible [ici](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html).

## Détails sur les modèles 3D

Lorsque le pattern est détecté par la caméra, il affiche un modèle hébergé sur ce repository GitHub ([lien URL](lien_url)). Comme pour de nombreux modèles 3D, les textures, l'éclairage et les UV sont appliqués via les fichiers annexes situés dans le dossier de chaque modèle. Explorez un modèle pour en savoir plus.

Cependant, le modèle est arbitraire en termes d'orientation, d'animation, de taille et de position. Toutes ces caractéristiques sont définies par les attributs passés dans la balise interne "a-marker", qui est la balise "a-entity".

Le modèle est à spécifier dans l'attribut "gltf-model", et le reste des attributs est décrit dans la documentation ainsi que de nombreux autres.

## Prochainement

Prochainement, vous pourrez télécharger depuis ce repository un livre PDF imprimable et assemblable destiné aux enfants pour leur faire découvrir de façon ludique différents animaux. Pour cela, rendez-vous sur le lien [ici](lien_pdf) et activez votre caméra.


 
