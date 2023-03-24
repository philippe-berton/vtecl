# Data visualization et jeux vidéos

# Introduction

## De quoi parle-t-on lorsque l'on dit "data visualization"?

La data visualization, ou visualisation de données, est l'utilisation de différentes méthodes pour résumer et montrer des liens entre des ensembles de données. Bien qu'avec le développement des big data et l'explosions des quantités de données disponibles les data visualization ont grandement évolués, celles-ci existent depuis le 18ème siècle. On a par exemple l'exemple suivant d'une visualisaton faite en 1869 par Charles Minard.

<p align="center">
  <img src="https://gallica.bnf.fr/ark:/12148/btv1b52504201x/f1.highres" height="500" />
</p>

Les visualisations sont aujourd'hui utilisées dans de nombreux domaines, et je me suis concentré lors de ma veille technologique avec son rapport aux jeux vidéos.

## Le rapport entre les data visualizations et les jeux vidéos

Le domaine des jeux vidéos est vaste et il existe différentes visualisation pour chaques catégories de jeux et chaque public visé. En effet le type de visualisation sera différent entre un jeu de tir en première personne et un jeu de stratégie en temps réel. De même, de manière claire, différentes visualisation sont utilisé en fonction du public cible, dépendament de si c'est un joueur jouant au jeu, un spectateur ou un joueur cherchant des ressources pour s'améliorer. En effet, l'e-sport s'est grandement développé ces dernières années et est aujourd'hui regardée par plus de 400 millions de personnes régulièrement [2]. Ce nombre de spectateur grandissant insite les développeurs des jeux à améliorer leurs mode spectateur, et également à développer des visualisation spécialement pour les grandes compétitions, qui ne sont disponibles que lors d'une retransmission. Ce développement de l'e-sport a également augmenté le nombre de joueur essayant de s'améliorer, que ce soit pour essayer de devenir professionnel, ou simplement pour une satisfaction personnelle. Ainsi un grand nombre de visualisation sont apparues pour suivre des statistiques sur ses parties ou sur les parties des autres joueurs, afin de faire progresser les joueurs souhaitant se renseigner sur le jeu.

# Un premier type de jeu : les First Person Shooter (FPS) à travers l'exemple de Counter-Strike:Global Offensive (CSGO)

## Pour un joueur

Dans les FPS classiques, les informations les plus intéressantes à avoir pour le joueur sont la quantité de point de vie qu'il possède et le nombre de balles qu'il a. On peut donc s'interesser à comment ces quantités sont donnés aux joueurs. 

Un article traitant de ce sujet a été publié en 2018 [1], des chercheurs ont fait une expériences avec des joueurs de jeux vidéos, et ont testés les performances de ceux ci, en utilisant différentes visualisation pour les point de vies et pour les munitions : 


<p align="center">
  <img src="https://ars.els-cdn.com/content/image/1-s2.0-S1875952117300435-gr6.jpg" height="100" />
</p>

Pour l'affichage des munition, c'est avec l'affichage (d) que les joueurs ont obtenu les meilleures performances. Cependant cet affichage n'est en général pas cohérent avec l'univers du jeu. On observe ainsi un dilemne apparaissant souvent dans le choix des data visualization pour les jeux vidéos, le dilemne **efficacité / immersion**.

Pour les FPS, le temps de réaction est très important, ainsi que le champ de vision du joueur. Les jeux actuel utilisent donc des HUD plutot simple, rapide à comprendre et on observe une uniformisation de ceux ci comme on le voit dans l'image suivante donnant les points de vie dans différents jeux : 

<p align="center">
  <img src="https://i.ibb.co/XDGC3St/image.png" height="100" />
</p>

Cette uniformisation est expliquée par l'efficacité de cette visualisation mais également car les joueurs sont habitués à ces affichages et s'habitueront donc plus facilement à un nouveau jeu si il reprend les codes existants. Au contraire, certains jeux choisissent de changer de style d'affichage ou même de supprimer certaines informations, voir toutes les informations disponibles afin d'avoir une immersion maximale ou de rendre le jeu plus difficile. 

## Les visualisation pour un spectateur

Pour les spectateurs, les informations peuvent être plus lentes à assimiler mais elles ne doivent pas l'empêcher de rater une action. Lors des rediffusion de parties, on a donc plus d'informations affichées, comme par exemple des informations sur tous les joueurs des deux équipes au lieu d'avoir uniquement les informations du joueur que l'on suit. D'autres visualisations plus complexes sont développés comme par exemple dans l'exemple de Counter strike : Global offensive, de nouveaux point de vue fixes ou mobiles, permettant de voir une action dans sa globalitée au lieu de suivre un joueur et de changer de joueur. On voit par exemple ci-après, la différence entre ce que voit un joueur et un spectateur dans la même situation (le spectateur à gauche et le joueur à droite).

<p align="center">
  <img src="https://i.ibb.co/VqSMz38/image.png" height="200" />
</p>

Aujourd'hui, ce sont des humains qui choisissent quel point de vue afficher pendant que d'autres humains commentent la partie. Cependant, cette méthode n'est pas suffisante lorsque les joueurs sont réparties sur toute la carte, et des actions sont régulièrements ratés par ces humains. Des chercheurs ont apporté une réponse en proposant d'utiliser de l'IA pour automatiser le déplacement du point de vue [3].

## Les visualisation en dehors du jeu

Les visualisation en dehors du jeu regroupent toutes les visualisations faites pour les joueurs ou autres personnes s'interessant à un jeu donné, qui aident ces personnes à comprendre le jeu ou à progresser sur celui ci. Ce sont celles-ci qui ressemblent le plus à des data visualization classique. Les informations peuvent être données par des sites tiers ou par les éditeurs du jeu vidéo, soit à l'aide d'API donnant un accès à des données du jeu et développés par l'éditeur, ou alors à l'aide de programmes tiers permettant de récupérer ces données [4]. Dans le cas de Counter strike : Global offensive, le site de référence dans ce domaine et csgostats.gg. Ce site permet aux utilisateurs de lier leurs comptes de jeu, puis de suivres les statistiques de leurs parties ou des parties des autres joueurs. Parmis les visualisations qu'ils proposent, on peut voir des dashboard contenant de nombreuses statistiques sur les parties d'un joueur : 

<p align="center">
  <img src="https://i.ibb.co/Z64B59m/image.png" height="200" />
</p>

Ou encore des heatmaps : 

<p align="center">
  <img src="https://i.ibb.co/1TRGhVK/image.png" height="280" />
</p>

Ces données permettent aux joueur de faire des bilans de leurs parties et de voir les erreurs qu'ils effectuent régulièrement. Un exemple très visuel et proche de visualisations plus traditionnelles est l'exemple des heatmaps précédentes. Sur ces heatmaps, on voit sur une carte, les positions où les joueurs éliminent un autre joueur et les positions où les joueurs se font éliminer. L'utilisateur peut ainsi, en regardant les statistiques sur l'ensemble des joueurs, voir les positions plutôt avantageuses et celles à éviter, et, en regardant les statistiques associés à leurs parties, ils peuvent voir quels endroit de la carte leur font défaut et sur lesquels ils doivent travailler. [4]

# Un deuxième type de jeu : les jeux massivement multijoueurs (MMORPG) à travers l'exemple de World of Warcraft

## Pour un joueur

Les MMORPG sont des jeux où le joueur fait progresser sont personnage et joue avec d'autres joueurs sur des sessions en général plus longues que pour un FPS. Contrairement Aux FPS, ce type de jeu n'est pas du tout développé au niveau de l'e-sport et n'a donc pas vraiment de visualisations faites pour les spectateurs. Cependant, contrairement aux FPS qui doivent laisser le contenu du jeu facilement et rapidement lisible, les MMORPG peuvent afficher des informations plus complexes, en cachant d'autres éléments du jeu. 

Ainsi, beaucoup de joueurs vont utiliser des "overlay", ce sont des logiciels tiers, qui vont modifier les données du jeu pour changer l'affichage du jeu, et ajouter des informations qui peuvent être utile au joueur. Pour les joueurs de plus haut niveaux, ces overlay sont si important qu'ils vont parfois utiliser la majorité de l'écran du joueur comme on peut le voir sur l'image suivante : 

<p align="center">
  <img src="https://i.ibb.co/6XVqMzK/image.png" height="280" />
</p>


Contrairement aux jeux FPS où les visualisations sont le plus souvent faites par des professionels, qu'elles soient destinées à être intégrées au jeu, à être vus par des spectateurs ou à aider les joueurs à progresser, dans les MMORPG, ce sont des joueurs qui créent la plupart des overlay pour améliorer l'expérience de jeu des autres joueurs.

## En dehors du jeu

Dans les MMORPG, les joueurs ont beaucoup d'activités' à faire en parallèle, ainsi la plupart des visualisation proposé hors jeu sont des outils de tracking pour suivre sa progression et ne pas être perdu dans ce qu'il reste au joueur à faire.



# Bibliographie

[1] : Peacocke, Margaree, Robert J. Teather, Jacques Carette, I. Scott MacKenzie, and Victoria McArthur. “An Empirical Comparison of First-Person Shooter Information Displays: HUDs, Diegetic Displays, and Spatial Representations.” Entertainment Computing 26 (May 1, 2018): 41–58. https://doi.org/10.1016/j.entcom.2018.01.003.


[2] : Nombre de téléspectateurs des événements d'esport dans le monde de 2019 à 2024, par engagement du téléspectateur : https://fr.statista.com/statistiques/1307153/audience-mondiale-esport/.

[3] : Joo, Ho-Taek, Sung-Ha Lee, Cheong-mok Bae, and Kyung-Joong Kim. “Learning to Automatically Spectate Games for Esports Using Object Detection Mechanism.” Expert Systems with Applications 213 (March 1, 2023): 118979. https://doi.org/10.1016/j.eswa.2022.118979.

[4] : Bowman, B., N. Elmqvist, and T. J. Jankun-Kelly. “Toward Visualization for Games: Theory, Design Space, and Patterns.” IEEE Transactions on Visualization and Computer Graphics 18, no. 11 (November 2012): 1956–68. https://doi.org/10.1109/TVCG.2012.77.

[5] : How does game stats tracker get players stats and display it on the website? : https://www.reddit.com/r/REGames/comments/gwt34s/how_does_game_stats_tracker_get_players_stats_and/.

[6] : Bucchieri, Federica, Yao, Lijie, and Isenberg, Petra. “Situated Visualization in Motion for Video Games,” 2022, 3 pages. https://petra.isenberg.cc/publications/papers/Bucchieri_2022_VIM-VideoGames.pdf.




