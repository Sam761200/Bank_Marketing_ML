# Projet de Machine Learning - Prédiction de Souscription à un Dépôt à Terme

Ce projet utilise un modèle de régression logistique pour prédire si un client va souscrire à un dépôt à terme en fonction des caractéristiques du client et des interactions précédentes avec la banque.

## Contenu

- `bank_marketing.ipynb` : Notebook contenant le code complet pour le chargement des données, le prétraitement, l'entraînement et l'évaluation du modèle.

## Description du Projet

Ce projet est basé sur le jeu de données "Bank Marketing" disponible sur l'[UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing). L'objectif est de prédire si un client souscrira (ou non) à un dépôt à terme (variable cible `y`).

### Étapes du Projet

1. **Importation des Bibliothèques** : Chargement des bibliothèques nécessaires pour la manipulation des données, la visualisation, la construction du modèle et l'évaluation.
2. **Chargement et Préparation des Données** : Chargement du jeu de données et affichage des premières lignes pour comprendre la structure des données.
3. **Exploration et Visualisation des Données** : Analyse rapide de la distribution de la variable cible.
4. **Prétraitement des Données** : Conversion des variables catégorielles en variables indicatrices, séparation des caractéristiques et de la variable cible, et standardisation des caractéristiques.
5. **Séparation des Données en Ensembles d'Entraînement et de Test** : Division des données en ensembles d'entraînement et de test.
6. **Construction et Entraînement du Modèle** : Création et entraînement d'un modèle de régression logistique.
7. **Évaluation du Modèle** : Utilisation des données de test pour évaluer les performances du modèle à l'aide de la matrice de confusion et du rapport de classification.
8. **Optimisation du Modèle** : Recherche par grille pour trouver les meilleurs hyperparamètres.

## Résultats

Les meilleurs hyperparamètres trouvés sont :
- **C = 1**
- **solver = 'liblinear'**

### Performance du Modèle

- **Matrice de Confusion** : 
  - Les valeurs diagonales (vraies prédictions positives et négatives) sont élevées, ce qui indique que le modèle prédit correctement la plupart des cas.
  - Les valeurs hors diagonales (faux positifs et faux négatifs) sont relativement faibles.
- **Rapport de Classification** :
  - Les scores de précision, rappel et F1 sont équilibrés et élevés pour les deux classes, indiquant une bonne performance globale du modèle.

## Instructions

1. Clonez le repository : `git clone https://github.com/vsam761200/Bank_Marketing_ML.git`
2. Ouvrez le notebook `bank_marketing.ipynb` dans Jupyter Notebook ou Google Colab.
3. Exécutez les cellules du notebook dans l'ordre pour reproduire les résultats.

## Contact

Pour toute question, veuillez contacter [samuel.saunier761200@gmail.com](mailto:samuel.saunier761200@gmail.com).
