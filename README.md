# Visualisation-de-données

A propos

Ce projet a été mené dans le cadre du cours de Visualisations des données à l’Université de Lausanne sous la direction de Monsieur Isaac Pante. Nous avons pour cela développé une visualisation à partir de la libraire JavaScript nommée D3.

Objectifs

Les réseaux sociaux font partie intégrante de notre quotidien. En effet, les pratiques sociales ont été largement modifiées par l’utilisation de ces derniers. Il nous a donc semblé légitime de développer un outil de visualisation pour quantifier le temps passé sur les différentes plateformes, à savoir, pour ce projet, Facebook, Instagram, Snapchat et Twitter.

Pour mener ce projet à bien, nous avons décidé de créer quatre curseurs désignant chacun un réseau social. Les curseurs indiquent la valeur approximative en heure passée sur le réseau en question.

La visualisation s’adapte en fonction de la modification de la valeur sélectionnée dans le curseur. Le chiffre à gauche du curseur, désignant le nombre d’heures, se met à jour automatiquement selon le positionnement de slider.

Plus le chiffre sélectionné est grand, plus l’ellipse représentant le temps passé sur le réseau social prend de l’ampleur. Plusieurs paramètres se modifient selon la force : la taille de l’ellipse et son opacité. Plus la valeur tend vers 0, plus la visualisation se fait petite jusqu’à disparaître si elle est à 0. A contrario, plus elle tend vers 24, plus elle prendra de l’ampleur jusqu’à atteindre son apogée lorsque la valeur 24 est sélectionnée.

Visualisations

 
Figure 1 - Curseurs

 
Figure 2 - Visualisation à la valeur par défaut (5)

 
Figure 3 - Les 4 visualisations à la valeur par défaut (5)

 
Figure 4 - Les 4 visualisations avec des valeurs différentes

Complications

Accès aux API
C’est avec regret que nous avons rencontré des difficultés pour récupérer les informations personnelles des utilisateurs. En effet, ce type de données restent grandement confidentielles et, par conséquent, une automatisation personnalisée des visualisations par extraction de données par utilisateur nous a été impossible.

Sliders dépendants

Améliorations

Lag

Responsive much ?
