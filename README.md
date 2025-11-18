# Encodeur_D-codeur_LSTM
# Traduction Anglais-Français avec Seq2Seq LSTM

Ce projet implémente un modèle **Seq2Seq** utilisant des **LSTM** pour la traduction automatique de l'anglais vers le français.

## Description

- Dataset : Paires de phrases anglais-français (~30 000 exemples)
- Prétraitement : Tokenisation, padding, ajout de tokens `<start>` et `<end>`
- Modèle : Encodeur–Décodeur avec Embedding + LSTM
- Entraînement : Jusqu'à 30 époques, batch size 64
- Evaluation : Prédictions qualitatives et courbes `loss` / `accuracy`

## Résultats

- Avec 15 000 exemples et 10 époques : traductions incohérentes  
- Avec 15 000 exemples et 30 époques : amélioration notable  
- Avec 30 000 exemples et 30 époques : traductions grammaticalement correctes et naturelles

## Usage

1. Charger le dataset `englishfrench.csv`
2. Exécuter le notebook `seq2seq_training.ipynb`
3. Observer les courbes d'entraînement et tester les traductions

## Références

- [English-French Dataset](https://drive.google.com/file/d/1OheJMYnZMLVEj4lwFEKL-3fogQkcY9Ae/view?usp=sharing)  
