# Visualisation-de-données

A propos

Ce projet a été mené dans le cadre du cours de Visualisations des données à l’Université de Lausanne sous la direction de Monsieur Pante. Nous avons pour cela développé une visualisation à partir de la libraire JavaScript nommée D3.

Objectifs

Les réseaux sociaux font partie intégrante de notre quotidien. En effet, les pratiques sociales ont été largement modifiées par l’utilisation de ces derniers. Il nous a donc semblé légitime de développer un outil de visualisation pour quantifier le temps passé sur les différentes plateformes, à savoir, pour ce projet, Facebook, Instagram, Snapchat et Twitter.

Pour mener ce projet à bien, nous avons décidé de créer quatre curseurs désignant chacun un réseau social. Les curseurs indiquent la valeur approximative en heure passée sur le réseau en question.

La visualisation s’adapte en fonction de la modification de la valeur sélectionnée dans le curseur. Le chiffre à gauche du curseur, désignant le nombre d’heures, se met à jour automatiquement selon le positionnement de slider.

Plus le chiffre sélectionné est grand, plus l’ellipse représentant le temps passé sur le réseau social prend de l’ampleur. Plusieurs paramètres se modifient selon la force : la taille de l’ellipse et son opacité. Plus la valeur tend vers 0, plus la visualisation se fait petite jusqu’à disparaître si elle est à 0. A contrario, plus elle tend vers 24, plus elle prendra de l’ampleur jusqu’à atteindre son apogée lorsque la valeur 24 est sélectionnée.

Visualisations

![alt text](https://raw.githubusercontent.com/fpham1/Visualisation-de-donn-es/master/Capture%20d%E2%80%99e%CC%81cran%202019-01-29%20a%CC%80%2016.14.29.png)
Figure 1 - Curseurs


Figure 2 - Visualisation à la valeur par défaut (5)


Figure 3 - Les 4 visualisations à la valeur par défaut (5)


Figure 4 - Les 4 visualisations avec des valeurs différentes

Complications

Accès aux API
C’est avec regret que nous avons rencontré des difficultés pour récupérer les informations personnelles des utilisateurs. En effet, ce type de données restent grandement confidentielles et, par conséquent, une automatisation personnalisée des visualisations par extraction de données par utilisateur nous a été impossible.

Sliders dépendants
La version précédente de notre code posait un problème fondamental dans la mesure où le premier slider (Facebook) agissait comme master des autres curseurs (Instagram, Snapchat et twitter). Cela avait pour effet que la valeur sélectionnée pour le curseur Facebook était reportée sur les autres curseurs et ne permettaient donc pas une visualisation indépendante pour chacun d’entre eux. Pour remédier à ce problème, nous avons recréé pour chaque slider des id différents.
Améliorations

Lag
En l’état, notre code affiche une visualisation qui souffre de lags. Par conséquent, une amélioration pertinente serait de cleaner le code afin de réctifier ce souci pour augmenter la fluidité de la visualisation. 

Responsive much ?
La responsivity de notre visualisation n’est pas parfaite. En effet, lors de la redimension de la fenêtre du navigateur, les visualisations s’adaptent par rapport à la largeur de cette dernière. Cependant, lors de la réactualisation de la page, les visualisations reprennent leur dimension d’origine à 100%. L’objectif serait donc d’implémenter un calcul qui permettrait de conserver les proportions lors de la redimension, même après le rafraîchissement de la page.
