# 🏥 AI pour la Détection des Maladies Cardiovasculaires

## Description  
Ce projet vise à prédire la présence de maladies cardiovasculaires en utilisant des techniques d'intelligence artificielle. Il comprend un prétraitement avancé des données et l'application de plusieurs modèles de machine learning pour optimiser les performances.  

## Prétraitement des données  
Afin d'améliorer la qualité des données et de garantir un bon équilibre des classes, les méthodes suivantes ont été appliquées :  
- **KNNImputer** pour l'imputation des valeurs manquantes.  
- **RobustScaler** pour normaliser les données et réduire l'effet des valeurs aberrantes.  
- **SMOTE (Synthetic Minority Over-sampling Technique)** pour équilibrer le dataset.  

## Modèles appliqués et performances  
Plusieurs modèles de machine learning ont été testés et comparés selon leur précision et leur rappel :  

| Modèle            | Accuracy | Recall  |
|------------------|----------|---------|
| Régression linéaire  | 0.565  | 0.612  |
| Decision Tree       | 0.737  | 0.907  |
| XGBoost            | 0.738  | 0.912  |
| AdaBoost           | 0.738  | 0.935  |
| RandomForest       | 0.746  | 0.907  |

📌 **Meilleurs modèles** :  
- **RandomForest** : Accuracy = **0.746**, Recall = **0.907**  
- **AdaBoost** : Accuracy = **0.738**, Recall = **0.935**  

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



