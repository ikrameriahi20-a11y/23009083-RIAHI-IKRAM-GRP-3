# F8 — Battre la marche aléatoire avec KNN

## Présentation du projet

Ce projet vise à étudier si l'algorithme K-Nearest Neighbors (KNN) peut prédire la direction du marché boursier américain le jour suivant, à partir des rendements historiques et de la volatilité passée du S&P 500.

L'objectif est de déterminer si KNN peut faire mieux qu'une prédiction naïve, appelée marche aléatoire dans le cadre de ce projet.

## Données utilisées

- **Source :** Federal Reserve Economic Data (FRED).
- **Série :** S&P 500 (`SP500`).
- **Lien :** https://fred.stlouisfed.org/series/SP500
- **Fichier :** `data/raw/SP500.csv`

## Méthodologie

Le projet utilise un modèle de classification K-Nearest Neighbors (KNN), associé à une normalisation des variables avec `StandardScaler`.

Les variables explicatives comprennent les rendements historiques décalés et des mesures de volatilité sur différentes périodes.

Les performances du modèle sont comparées à celles d'un modèle de référence naïf (`DummyClassifier`).

## Organisation du dépôt

- `data/` : données utilisées dans le projet.
- `docs/` : fiche du sujet et références.
- `notebooks/` : notebook principal.
- `figures/` : graphiques générés.
- `rapport/` : rapport final.
- `presentation/` : présentation du projet.

## Exécution

Installer les dépendances :

```bash
pip install -r requirements.txt
```

Ouvrir ensuite le notebook `notebooks/projet_F8.ipynb` avec Jupyter ou Google Colab.

## Algorithme utilisé

K-Nearest Neighbors (KNN), avec recherche des meilleurs hyperparamètres par validation croisée temporelle.

## Auteurs

À compléter.

