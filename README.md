# Analyse des départs de clients d'une banque (churn) — Projet d'équipe (Équipe 9)

## Problématique
Comprendre et anticiper l'attrition (churn) des clients d'une institution bancaire à partir de données historiques, afin d'orienter des actions de fidélisation.

## Données
Données clients d'une banque (voir `Code Final Equipe 9.Rmd` et les rapports inclus pour le détail des variables). Les valeurs manquantes ont été traitées par imputation multiple (package `mice`).

## Méthode
- Analyse exploratoire approfondie (EDA) et tests de dépendance entre variables pour identifier les facteurs associés au départ des clients
- Comparaison de six modèles de classification :
  - Classificateur naïf de Bayes (Naive Bayes)
  - Analyse linéaire discriminante (ALD)
  - Régression logistique
  - K-Nearest Neighbour (KNN)
  - Arbre de décision
  - XGBoost (Extreme Gradient Boosting)
- Évaluation de chaque modèle sur trois critères complémentaires (précision, sensibilité, spécificité) pour tenir compte du déséquilibre des classes
- Validation croisée (`e1071`) et courbes ROC (`ROCR`)

## Résultats
Le meilleur modèle a été sélectionné selon les critères ci-dessus ; voir les rapports inclus (`Rapport Final Equipe 9.pdf` et `.docx`) pour le détail des résultats et les recommandations de fidélisation client. Une démonstration vidéo a été réalisée en local lors de la présentation du projet (non incluse dans ce dépôt en raison de sa taille de plus de 140 Mo ; peut être ré-enregistrée si besoin).

## Reproduire
```bash
Ouvrir le fichier "Code Final Equipe 9.Rmd" dans RStudio et faire Knit
(packages requis : MASS, readxl, tidyverse, caret, FNN, mice, FactoMineR, e1071, klaR, ROCR, class, kknn)
```
