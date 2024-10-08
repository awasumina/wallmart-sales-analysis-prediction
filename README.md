# Wallmart Sales Prediction Analysis

## Overview

This project aims to analyze and predict  sales for a wallmart store using various machine learning techniques. The analysis focuses on understanding the key factors affecting sales and evaluating different regression models for prediction accuracy.

## Methodology

1. **Data Preprocessing**:
   - The dataset was cleaned and preprocessed, removing any unnecessary columns that did not contribute significantly to the model's performance.
   - Categorical variables were encoded as needed.

2. **Feature Importance**:
   - Used Random Forest Regressor to identify important features affecting weekly sales.
   - Visualized feature importances using a horizontal bar plot.

3. **Model Selection and Evaluation**:
   - Split the data into training and testing sets using `train_test_split`.
   - Implemented multiple regression models:
     - **Decision Tree Regressor**
     - **Random Forest Regressor**
     - **XGBoost Regressor**
     - **Ridge Regression** (for regularization to prevent overfitting)
   - Evaluated models using metrics such as R² score, Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).

## Results

- **Feature Importance**:
   - Visual representation of feature importances revealed that factors such as `Temperature`, `Fuel_Price`, and `Size` significantly impacted weekly sales.
  
- **Model Performance**:
   - **Decision Tree Regressor**:
     - R² score: 0.38
     - RMSE: 17977.34
   - **Random Forest Regressor**:
     - R² score: 0.38
     - RMSE: 7760.75
   - **XGBoost Regressor**:
     - R² score: 0.91
     - RMSE: 6799.06
   - **Ridge Regression**:
     - Maintained similar performance metrics as the XGBoost model.

The XGBoost model exhibited the highest accuracy in predicting weekly sales, indicating it as the best model for this analysis.

## Conclusions

This analysis highlights the significant influence of environmental and economic factors on weekly sales performance in retail. The models' performance indicates that machine learning techniques, especially ensemble methods like XGBoost, can effectively predict sales, allowing retailers to make informed decisions based on predictive insights.
