Projet de Classification de Feuilles (Leaf Classificiation)
============================================================

## Aperçu

Ce projet vise à résoudre le problème de classification de feuilles en utilisant six modèles de classification différents. Chaque modèle est conçu pour prédire la classe d'une feuille sur la base de caractéristiques spécifiques extraites de l'image de la feuille.

## Données

Les données utilisées pour l'entraînement et les tests sont stockées dans le dossier 'data'.
Le jeu de données comprend environ 1 584 images de spécimens de feuilles (16 échantillons de chacune des 99 espèces), converties en feuilles noires binaires sur fond blanc. Trois ensembles de caractéristiques sont également fournis par image : un descripteur continu de forme, un histogramme de texture intérieure et un histogramme de marge à petite échelle. Pour chaque caractéristique, un vecteur de 64 attributs est donné par échantillon de feuille.


Les colonnes du jeu de données sont les suivantes :
- `id` : un identifiant anonyme unique pour une image
- `margin_1`, `margin_2`, ..., `margin_64` : chacun des 64 vecteurs d'attributs pour la caractéristique de marge
- `shape_1`, `shape_2`, ..., `shape_64` : chacun des 64 vecteurs d'attributs pour la caractéristique de forme
- `texture_1`, `texture_2`, ..., `texture_64` : chacun des 64 vecteurs d'attributs pour la caractéristique de texture

Pour plus de détails sur les données, veuillez consulter la [source des données sur Kaggle](https://www.kaggle.com/c/leaf-classification/data).

## Modèles de Classification


1. **Modèle 1 - Support Vector Machine (SVM) :** Description du modèle et de ses caractéristiques.

2. **Modèle 2 - Réseau de Neurones Convolutifs (CNN) :** Description du modèle et de ses caractéristiques.

3. **Modèle 3 - K-Nearest Neighbors (KNN) :** Description du modèle et de ses caractéristiques.

4. **Modèle 4 - Random Forest :** Description du modèle et de ses caractéristiques.

5. **Modèle 5 - Gradient Boosting :** Description du modèle et de ses caractéristiques.

6. **Modèle 6 - Régression Logistique :** Description du modèle et de ses caractéristiques.

## Données
Les données utilisées pour l'entraînement et les tests sont stockées dans le dossier `data`. Assurez-vous de fournir des détails sur la source des données et leur format.

## Installation
1. Clonez le dépôt GitHub sur votre machine locale.
   ```bash
   git clone https://github.com/votre-utilisateur/nom-du-projet.git
