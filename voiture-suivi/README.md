# Suivi électrique — Opel Corsa-e

Petit tableau de bord statique pour suivre les recharges et la consommation de la Corsa-e.

## Fonctionnalités
- saisie de chaque recharge : date, compteur, kWh, coût, domicile/extérieur et température ;
- calcul automatique de la distance entre deux relevés ;
- consommation en kWh/100 km ;
- comparaison mensuelle des coûts domicile / extérieur ;
- graphique kilomètres + coûts + consommation ;
- nuage de points température / consommation ;
- historique des recharges ;
- export et import CSV ;
- stockage local dans le navigateur, sans serveur ni compte.

## Utilisation
L'application est indépendante du reste du dépôt et se trouve dans 'voiture-suivi/'.

Avec GitHub Pages sur la branche 'main', elle est accessible à :
https://Cufflink9705.github.io/evenements-alboussiere/voiture-suivi/

Les données saisies ne sont pas écrites dans GitHub : elles restent dans le stockage local du navigateur. L'export CSV permet de conserver une sauvegarde.

## Calcul
Pour une recharge, la distance est la différence entre son compteur et celui de la recharge précédente. La consommation de la période est : kWh chargés / kilomètres parcourus × 100.

La première recharge ne produit donc pas encore de consommation calculée. Plus les relevés sont réguliers, plus les graphiques deviennent utiles.

## Isolation
Le projet n'utilise aucun fichier, workflow ou configuration du système de veille événementielle. Il est contenu dans son propre dossier.
