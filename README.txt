


Nous avons implémenté un algorithmes AlphaBeta avec du "iterative deepening" pour gérer le temps et pouvoir terminer la partie dans le temps imparti

On a supposé qu'on joue un peu près 60 coups par partie, et on a réparti notre temps uniformément entre les coups joués

L'heuristique utilisé repose sur 3 techniques :
    1. La première associe à chaque case du tableau de jeu un score. Les cases stratégique ayant un meilleur score comme les coins du tableau de jeu
    2. le nombre de pièce dans la table de jeu
    3. la mobilité du joueur , c'est à dire le nombre de coups qu'il peut jouer

en parrallèle avec l'iterative deepening, on a essayé de trier les fils de la racine selon leur évaluation heuristique avant de lancer l'algorithme de alpha AlphaBeta
Cette technique avait pour but de rendre l'algo alpha beta beaucoup plus efficace dans l'élagage de l'arbre de recherche

Une table de hachage a été implémenté pour y stocker les évaluations des boards pour ne pas avoir à les calculer une autre fois
Seul le hash du board est stocké dans la table de hachage. La fonction de hachage repose sur le hachage de Zobrist
On a pas eu le temps de bien implémenter cette dernière technique, mais un pas vers ce sens à été réalisé
