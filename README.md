# AI for Gamma Telescope Classification

## Description
Ce projet vise à classifier les données issues des télescopes gamma en utilisant des techniques d'intelligence artificielle. Il inclut un prétraitement avancé des données et l'application de plusieurs modèles de machine learning pour obtenir des performances optimales.

## Prétraitement des données
Afin d'assurer une meilleure qualité des données et d'équilibrer la distribution des classes, les techniques suivantes ont été employées :
- **SMOTE (Synthetic Minority Over-sampling Technique)** pour équilibrer le dataset.
- **Yeo-Johnson Transformation** pour normaliser les données.
- **RobustScaler** pour réduire l'impact des valeurs aberrantes.

## Modèles appliqués et performances
Plusieurs modèles de machine learning ont été testés et comparés en fonction de leur précision, rappel et exactitude :

| Modèle                  | Accuracy  | Precision | Recall   |
|--------------------------|-----------|-----------|-----------|
| Logistic Regression      | 0.800357  | 0.807610  | 0.788597  |
| Decision Tree           | 0.835104  | 0.864331  | 0.795166  |
| Extreme Gradient Boosting | 0.885907  | 0.903201  | 0.864497  |
| Gradient Boosting       | 0.814426  | 0.811462  | 0.819330  |
| Random Forest          | 0.895921  | 0.905862  | 0.883715  |
| Support Vector Machine | 0.895557  | 0.879117  | 0.917124  |

## Installation
### Prérequis
- Python 3.x
- Bibliothèques Python suivantes :
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `imbalanced-learn`
  - `xgboost`
  - `matplotlib`
  - `seaborn`

### Installation des dépendances
```bash
pip install pandas numpy scikit-learn imbalanced-learn xgboost matplotlib seaborn
```

## Utilisation
1. Charger les données et appliquer les techniques de prétraitement.
2. Entraîner les modèles et évaluer leurs performances.
3. Comparer les résultats pour choisir le modèle optimal.

## Auteurs
Ce projet a été réalisé dans le cadre d'un projet de fin d'études sous la supervision de **M. Abdelkarim El Mouatasim**.

## Licence
Ce projet est sous licence MIT - voir le fichier LICENSE pour plus de détails.

