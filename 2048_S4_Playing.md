# Fonctionnalité 6 : Mettre en orchestre le jeu

Nous arrivons maintenant presque au bout de notre MVP. Il s'agit maintenant de mettre en orchestre le déroulé du jeu. Pour cette fonctionnalité, on va aussi procéder en différentes étapes. 


# Etape 1 : faire jouer l'ordinateur de manière aléatoire.

Il s'agit de lancer une partie avec l'ordinateur jouant à la place du joueur et votre programme doit donc consister en :

 + Initialiser une grille de jeu, les paramètres du jeu étant les paramètres par défaut.
 + L'afficher
 + Mettre en place une boucle permettant de mettre en oeuvre les actions suivantes si le jeu n'est pas terminé
 	+ Choisir un mouvement possible de manière aléatoire
 	+ Appliquer ce mouvement sur la grille
 	+ Ajouter une nouvelle tuile
 	+ Affichage de la grille
 + Tester si la configuration obtenue à la fin du jeu est une configuration gagnante.

 
 Avez-vous l'ensemble des éléments dans ce que vous avez déjà réalisé pour mettre en place ce programme de jeu ?
 
 Si oui, ecrivez la fonction `random_play()` qui met en oeuvre ce jeu.
 
 
# Etape 2 : Permettre la configuration du jeu  

On souhaite permettre à l'utilisateur le choix sur la taille de la grille de départ ainsi que sur le thème souhaité. Pour cela, écrire les fonctions:

+  `ask_and_read_grid_size()`
+   `ask_and_read_grid_theme()`

qui permettent de demander et de saisir les choix de l'utilisateur.



# Etape 3 : Faire jouer le joueur
 
Il s'agit maintenant de permettre à un joueur de jouer. Il s'agit donc d'écrire la fonction `game_play()` qui :

+ Demande à l'utilisateur de choisir une taille et un thème de grille.  
+ Initialise une grille de jeu qui respectent les paramètres demandés.
+ L'affiche
+ Met en place une boucle permettant de mettre en oeuvre les actions suivantes si le jeu n'est pas terminé
	+ Demande à l'utilisateur de saisir son choix de direction
	+ Applique ce mouvement sur la grille
	+ Ajoute une nouvelle tuile
	+ Affiche la grille obtenue
+ Teste si la configuration obtenue à la fin du jeu est une configuration gagnante.


# Etape 4 : Lancer le jeu

La dernière étape pour finir cette fonctionnalité est de lancer le jeu. Pour cela il faut donc ajouter une fonction principale dans votre fichier `textual_2048.py` 

```PYTHON
if __name__ == '__main__':
    game_play()
    exit(1)  
```

A ce stade, nous avons terminé notre objectif 1 et nous avons donc notre MVP pour le jeu 2048.
Avant de passer à la suite et de mettre à jour votre dépôt git, nous vous demandons de bien prendre le temps d'ajouter un maximum de tests unitaires à votre projet (si vous avez appliqué la méthodologie TDD, cela ne devrait pas vous prendre trop de temps) et de commenter vos différentes fonctions. 


# Etape 5 : Retours utilisateurs sur votre jeu

A ce stade, nous allons aussi essayer d'avoir des retours utilisateurs sur ce MVP. Vous allez donc prendre ce role et et tester votre jeu en jouant avec. Chaque membre du binome peut par exemple faire une partie.

Quels sont vos retours utilisateurs sur ce MVP ? Y-a-t'il des fonctionnalités manquantes et que vous aimeriez ajouter à votre projet.

Prenez-le temps d'en discuter en binome et plus globalement avec la totalité du groupe afin de lister les fonctionnalités que vous aimeriez ajouter à votre jeu. Donner leur aussi une priorité.

Suite à ce brainstorming, vous ajouterez un fichier `TO_DO.txt` (ou `TO_DO.md`) à votre projet dans lequel vous listerez, par ordre de priorité, ces différentes fonctionnalités.


## Pour finir 

+ <span style='color:blue'>Faire un commit de vos derniers changements.</span> 
+ <span style='color:blue'>Tagger ce dernier commit </span> 
+ <span style='color:blue'>Pousser (Push) votre code vers votre dépôt distant sur GitLab.</span> 
+ <span style='color:blue'>Faire un test de couverture de code de votre MVP et pousser le bilan obtenu vers votre dépôt distant sur GitLab.</span>


Et on peut maintenant passer à l'[objectif 2](./TemplateProject_2048.md). 






