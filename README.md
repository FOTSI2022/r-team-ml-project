# Projet d'équipe - Machine Learning (Équipe 9)

## Problématique
Projet d'équipe de modélisation prédictive visant à comparer plusieurs approches de machine learning (notamment la régression KNN et des méthodes de classification) sur un jeu de données, avec gestion des valeurs manquantes par imputation.

## Données
Jeu de données utilisé dans `Code Final Equipe 9.Rmd` (voir le rapport pour le détail complet des variables). Les données manquantes ont été traitées par imputation multiple (package `mice`).

## Méthode
- Importation et préparation des données (`readxl`, `mice` pour l'imputation des valeurs manquantes)
- Analyse exploratoire et statistiques descriptives
- Modélisation par régression KNN (`FNN`, `kknn`) et autres méthodes de classification (`MASS`, `caret`, `class`, `klaR`)
- Analyse en composantes principales (`FactoMineR`) et validation croisée (`e1071`)
- Évaluation des modèles par courbes ROC (`ROCR`)

## Résultats
Voir les rapports inclus (`Rapport Final Equipe 9.pdf` et `.docx`) pour le détail des résultats et conclusions de l'équipe. Une démonstration vidéo a été réalisée en local lors de la présentation du projet (non incluse dans ce dépôt en raison de sa taille de plus de 140 Mo ; peut être ré-enregistrée si besoin).

## Reproduire
```bash
Ouvrir le fichier "Code Final Equipe 9.Rmd" dans RStudio et faire Knit
(packages requis : MASS, readxl, tidyverse, caret, FNN, mice, FactoMineR, e1071, klaR, ROCR, class, kknn)
```
