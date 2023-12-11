Projet de Classification de Feuilles (Leaf Classificiation)
============================================================

## Aperçu

ce projet vise à résoudre le défi de classification des feuilles en exploitant six modèles distincts de classification. Chaque modèle est élaboré afin de prédire la catégorie d'une feuille en se fondant sur des caractéristiques spécifiques extraites.

## Structure du Projet

    ├── data/
    │   ├── train.csv
    │   ... 
    ├── src/
    │   ├── __init__.py
    │   ├── Classify_Data.py
    │   ├── Preprocess_Data.py
    │   ├── Visualize_Results.py
    │   ... 
    ├── requirements.txt
    ├── projet.ipynb
    ├── LICENSE
    ├── AUTHORS.rst
    ├── .editorconfig
    ├── Makefile
    ├── .travis.yml
    ├── .gitignore
    └── README.md

La structure du projet est organisée comme suit :

- **data/** : Répertoire contenant les données du projet, avec notamment le fichier `train.csv`.

- **src/** : Répertoire abritant les scripts source du projet :
  - **_init_.py** : Fichier d'initialisation du module Python.
  - **Classify_Data.py** : Script pour la classification des données.
  - **Preprocess_Data.py** : Script pour le prétraitement des données.
  - **Visualize_Results.py** : Script pour la visualisation des résultats.
  - ...

- **requirements.txt** : Fichier spécifiant les dépendances du projet.

- **projet.ipynb** : Fichier Jupyter Notebook contenant le code principal du projet.

- **LICENSE** : Fichier décrivant la licence du projet.

- **AUTHORS.rst** : Fichier listant les auteurs du projet.

- **.editorconfig** : Fichier de configuration pour les éditeurs de texte.

- **Makefile** : Fichier utilisé pour automatiser des tâches dans le projet.

- **.travis.yml** : Fichier de configuration pour l'intégration continue avec Travis CI.

- **.gitignore** : Fichier spécifiant les fichiers et répertoires à ignorer lors du suivi avec Git.

- **README.md** : Fichier que vous êtes actuellement en train de lire, contenant des informations générales sur le projet.


## Données

Les données destinées à l'entraînement et aux tests sont consignées dans le répertoire `data`. Le corpus de données en question compte approximativement 991 entrées.

Les colonnes contenues dans le jeu de données sont définies comme suit :
- `id` : un identifiant anonyme unique pour une image
- `margin_1`, `margin_2`, ..., `margin_64` : chacun des 64 vecteurs d'attributs pour la caractéristique de marge
- `shape_1`, `shape_2`, ..., `shape_64` : chacun des 64 vecteurs d'attributs pour la caractéristique de forme
- `texture_1`, `texture_2`, ..., `texture_64` : chacun des 64 vecteurs d'attributs pour la caractéristique de texture

Pour plus de détails sur les données, veuillez consulter la [source des données sur Kaggle](https://www.kaggle.com/c/leaf-classification/data).

## Modèles de Classification

1. **Modèle 1 - Régression Logistique :** La régression logistique est un modèle de classification utilisé pour prédire la probabilité qu'une observation appartienne à une catégorie particulière. Elle fonctionne en ajustant une courbe logistique aux données d'entraînement. [Documentation de la Régression Logistique](https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression)

2. **Modèle 2 - Support Vector Classification (SVC) :** Le modèle de classification par machine à vecteurs de support (SVC) cherche à séparer les classes en trouvant le meilleur hyperplan qui maximise la marge entre les différentes classes. [Documentation du SVC](https://scikit-learn.org/stable/modules/svm.html#classification)

3. **Modèle 3 - SGD (Stochastic Gradient Descent) :** Le SGD est un algorithme d'optimisation utilisé dans le contexte de la classification. Il ajuste les paramètres du modèle en utilisant la descente de gradient sur des échantillons aléatoires. [Documentation du SGD](https://scikit-learn.org/stable/modules/sgd.html)

4. **Modèle 4 - Random Forest :** Random Forest est un ensemble d'arbres de décision où chaque arbre vote pour une classe et la classe majoritaire est choisie. Cela améliore la robustesse et la précision du modèle. [Documentation du Random Forest](https://scikit-learn.org/stable/modules/ensemble.html#random-forests)

5. **Modèle 5 - Adaboost :** Adaboost est un modèle de boosting qui combine plusieurs modèles faibles pour former un modèle fort. Il assigne des poids aux observations, donnant plus d'importance aux erreurs précédentes. [Documentation de l'Adaboost](https://scikit-learn.org/stable/modules/ensemble.html#adaboost)

6. **Modèle 6 - Bagging :** Le bagging (Bootstrap Aggregating) est une technique d'ensemble où plusieurs modèles sont entraînés sur différents sous-ensembles des données d'entraînement. Cela réduit la variance du modèle global. [Documentation du Bagging](https://scikit-learn.org/stable/modules/ensemble.html#bagging-meta-estimator)

## Installation
1. Clonez le dépôt GitHub sur votre machine locale.
   ```bash
   git clone https://github.com/votre-utilisateur/nom-du-projet.git
Guide d'Installation
Prérequis
Python (version 3.x recommandée)
Git (pour cloner le dépôt)
Étapes d'Installation
Clonez le Dépôt

bash
Copy code
git clone https://github.com/votre-utilisateur/nom-du-projet.git
cd nom-du-projet
Créez un Environnement Virtuel (Optionnel)

bash
Copy code
python -m venv venv
source venv/bin/activate   # Pour Linux/Mac
# ou
.\venv\Scripts\activate    # Pour Windows
Installez les Dépendances

bash
Copy code
pip install -r requirements.txt
Exécutez le Projet

Entraînez les modèles et effectuez les prédictions.
bash
Copy code
python projet.ipynb
Remarques
Assurez-vous que l'environnement virtuel est activé avant d'installer les dépendances ou d'exécuter le projet.
Le fichier projet.ipynb peut être exécuté dans un environnement Jupyter Notebook ou dans tout autre environnement compatible avec les notebooks.
Pour des détails spécifiques sur l'utilisation du projet, consultez la section "Utilisation" dans le fichier README.md.
* Free software: MIT license

