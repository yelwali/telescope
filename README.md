# 🏥 AI for Gamma Telescope Classification
Ce projet vise à classer les événements détectés par un télescope gamma en utilisant différentes techniques d'apprentissage automatique. L'objectif est de distinguer les signaux gamma (classe positive) du bruit de fond (classe négative) avec une précision élevée.

## Pré-traitement des données

1. **Normalisation des données** : 
   - Les données numériques ont été normalisées en utilisant le `RobustScaler` pour réduire l'effet des valeurs aberrantes.
   - Une transformation de normalisation supplémentaire a été appliquée avec `PowerTransformer` (méthode Yeo-Johnson) pour stabiliser la variance et rendre les données plus gaussiennes.

2. **Équilibrage des classes** :
   - Le déséquilibre des classes a été corrigé en utilisant la technique **SMOTE** (Synthetic Minority Over-sampling Technique). Cela permet de générer des échantillons synthétiques pour la classe minoritaire, améliorant ainsi la performance des modèles sur cette classe.

## Modèles utilisés et résultats

Plusieurs modèles d'apprentissage automatique ont été entraînés et évalués sur le dataset. Voici un résumé de leurs performances :

| Modèle                        | Accuracy | Precision | Recall |
|-------------------------------|----------|-----------|--------|
| Logistic Regression           | 0.800357 | 0.807610  | 0.788597 |
| Decision Tree                 | 0.835104 | 0.864331  | 0.795166 |
| Extreme Gradient Boosting     | 0.885907 | 0.903201  | 0.864497 |
| Gradient Boosting             | 0.814426 | 0.811462  | 0.819330 |
| Random Forest                 | 0.895921 | 0.905862  | 0.883715 |
| Support Vector Machine (SVM)  | 0.895557 | 0.879117  | 0.917124 |

### Analyse des résultats
- **Random Forest** et **SVM** ont obtenu les meilleures performances en termes d'**Accuracy** et de **Recall**.
- **Extreme Gradient Boosting** a également montré des résultats compétitifs, avec une précision élevée.
- **Logistic Regression** et **Gradient Boosting** ont des performances légèrement inférieures mais restent acceptables.

## Conclusion
Le modèle **Random Forest** semble être le meilleur choix pour ce projet, offrant un bon équilibre entre précision et rappel. Cependant, le **SVM** pourrait être préféré si le rappel est une métrique plus critique pour l'application.

## Prochaines étapes
- Explorer l'optimisation des hyperparamètres pour améliorer davantage les performances.
- Tester des architectures de réseaux de neurones pour comparer avec les modèles traditionnels.
- Déployer le modèle sélectionné dans un environnement de production pour une classification en temps réel.

## Dépendances
- Python 3.x
- Bibliothèques : `scikit-learn`, `imbalanced-learn`, `pandas`, `numpy`, `xgboost`

## Installation
1. Cloner le dépôt :
   ```bash
   git clone https://github.com/votre-utilisateur/ai-gamma-telescope.git

```

## Utilisation
1. Charger les données et appliquer les techniques de prétraitement.
2. Entraîner les modèles et évaluer leurs performances.
3. Comparer les résultats pour choisir le modèle optimal.

## Auteurs
Ce projet a été réalisé dans le cadre d'un projet de fin d'études sous la supervision de **M. Abdelkarim El Mouatasim**.

## Licence
Ce projet est sous licence MIT - voir le fichier LICENSE pour plus de détails.



