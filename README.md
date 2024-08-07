# Machine Learning Assignment - Predicting Fruit Fly Sex

## Overview

This project aims to predict the sex of fruit flies based on various physical characteristics using different machine learning models. The dataset contains 1731 rows and 20 columns, representing the measurements and features of individual fruit flies.

## Dataset

- **Source**: "83_Loeschcke_et_al_2000_Thorax_&_wing_traits_lab pops.csv"
- **Columns**: Geography, sex, and various measurements
- **Target Variable**: Sex (1 for male, 0 for female)

## Models Used

1. **Linear Regression**
   - Baseline model
   - Used Ridge and Lasso regularization
   - Compared performance with and without PCA

2. **Random Forest**
   - Evaluated the impact of dimensionality reduction (PCA)
   - Hyperparameter tuning using RandomizedSearchCV

3. **K Nearest Neighbor (KNN)**
   - Compared performance with and without PCA
   - Hyperparameter tuning using GridSearchCV

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- Log Loss
- ROC Curve and AUC

## Results

- **Linear Regression**
  - Non-PCA: Accuracy of 93.8%
  - PCA: Accuracy of 92.2%
  - Ridge and Lasso improved model performance

- **Random Forest**
  - Non-PCA: Accuracy of 93.2%
  - PCA: Accuracy of 93.8%
  - Best performance after hyperparameter tuning: 93.9%

- **K Nearest Neighbor (KNN)**
  - Non-PCA: Accuracy of 93.2%
  - PCA: Accuracy of 92.8%
  - Best performance after hyperparameter tuning: 92.7%

## Conclusion

The Random Forest model with hyperparameter tuning provided the highest accuracy for predicting the sex of fruit flies. This project demonstrates the importance of model selection, feature engineering, and hyperparameter tuning in achieving optimal performance.
