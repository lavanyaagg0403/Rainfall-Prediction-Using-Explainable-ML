# Rainfall Prediction Using Explainable Machine Learning

## Overview

This project uses machine learning to predict daily rainfall from historical weather data for Indian cities. A Random Forest Regressor is used for rainfall prediction, and SHAP (SHapley Additive exPlanations) is used to examine how individual features contribute to the model's predictions.

The project covers data preprocessing, exploratory analysis, feature engineering, model training, evaluation, feature importance analysis, and model interpretation.

## Dataset

The project uses daily weather data covering the period from 2000 to 2024.

The dataset contains weather-related variables such as:

- City
- Date
- Maximum temperature
- Minimum temperature
- Apparent temperature
- Weather code
- Wind speed
- Wind gusts
- Wind direction
- Rainfall

The target variable is daily rainfall.

## Methodology

The following steps were performed:

1. Loaded and examined the weather dataset.
2. Performed data preprocessing and handled the required data transformations.
3. Extracted date-related features such as year, month, and day.
4. Selected the weather variables used for prediction.
5. Split the data into training and testing sets.
6. Trained a Random Forest Regression model.
7. Evaluated the model using MAE, RMSE, and R².
8. Examined the feature importance provided by the Random Forest model.
9. Applied SHAP to examine the contribution of individual features to model predictions.
10. Used SHAP summary, feature importance, and waterfall plots for model interpretation.

## Model

### Random Forest Regressor

A Random Forest Regressor was selected to predict daily rainfall. Random Forest can model nonlinear relationships between the input weather variables and rainfall.

The model was evaluated on the test dataset using the following metrics:

| Metric | Value |
|---|---:|
| MAE | 1.091 |
| RMSE | 3.799 |
| R² | 0.820 |

These values correspond to the current model configuration and test split used in the notebook.

## Explainability

SHAP was used to examine how the trained Random Forest model arrives at its predictions.

Three types of SHAP visualizations are included in the notebook:

### SHAP Summary Plot

The summary plot shows the contribution of the input features across a representative sample of test observations. It provides information about both the magnitude and direction of feature contributions.

### SHAP Feature Importance

The SHAP feature importance plot ranks features according to their average contribution magnitude to the model's predictions.

### SHAP Waterfall Plot

The waterfall plot explains an individual prediction by showing how the feature contributions move the prediction from the model's baseline value to the final predicted value.

For the individual example included in the notebook:

- Actual rainfall: 26.40
- Predicted rainfall: 27.98

The SHAP explanation was checked by reconstructing the prediction from the SHAP base value and feature contributions. The reconstructed value matched the model prediction within floating-point precision.

The SHAP analysis is used to explain the behavior of the trained model. The feature contributions should not be interpreted as evidence of causal relationships.

## Visualizations

The notebook contains the following visualizations:

- Rainfall distribution
- Average rainfall by city
- Correlation heatmap
- Actual vs. predicted rainfall
- Random Forest feature importance
- SHAP summary plot
- SHAP feature importance plot
- SHAP waterfall plot

## Repository Structure

```text
Rainfall-Prediction-Using-Explainable-ML/
│
├── README.md
├── Rainfall_Prediction_Using_Random_Forest.ipynb
├── requirements.txt
├── .gitignore
├── LICENSE
└── images/

## Requirements

The project uses Python and the following libraries:

pandas
numpy
matplotlib
seaborn
scikit-learn
shap

The required packages are listed in requirements.txt.

## Running the Project

The notebook can be run using Google Colab or a local Jupyter environment.

1.Clone or download the repository.
2.Install the packages listed in requirements.txt.
3.Open Rainfall_Prediction_Using_Random_Forest.ipynb.
4.Provide the required dataset when prompted.
5.Run the notebook cells sequentially.

## Future Work
 Possible extensions include:
-Hyperparameter tuning of the Random Forest model
-Comparison with other regression models
-Cross-validation
-Evaluation across individual cities
-Integration of additional weather variables
-Development of a rainfall prediction interface

## Author

Lavanya Aggarwal

B.Tech Computer Science Engineering
Amity University Noida

GitHub: https://github.com/lavanyaagg0403
