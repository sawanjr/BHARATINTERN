
markdown
# Wine Quality Prediction using Linear Regression

This Jupyter Notebook was created as part of my internship program provided by BhartIntern. The task assigned was to build a Machine Learning model to predict the quality of wine using linear regression.

## Background Knowledge

The dataset used in this project contains information about red variants of the Portuguese "Vinho Verde" wine. Here are the columns and their descriptions:

- **Fixed Acidity**: Most acids involved with wine, or fixed/nonvolatile.
- **Volatile Acidity**: The amount of acetic acid in wine, affecting taste.
- **Citric Acid**: Found in small quantities, adding freshness and flavor.
- **Residual Sugar**: Amount of sugar remaining after fermentation.
- **Chlorides**: The amount of salt in the wine.
- **Free Sulfur Dioxide**: Prevents microbial growth and oxidation.
- **Total Sulfur Dioxide**: Amount of free and bound forms of sulfur dioxide.
- **Density**: Density of the wine.
- **pH**: Describes how acidic or basic the wine is.
- **Sulphates**: Wine additive contributing to sulfur dioxide gas.
- **Alcohol**: Alcohol content of the wine.
- **Quality**: The quality score of the wine (target variable).

## Libraries Used


-import numpy as np
-import pandas as pd
-from matplotlib import pyplot as plt
-import seaborn as sns

# Importing the dataset
df = pd.read_csv("winequality-red.csv")


## Data Exploration

- The dataset contains 1599 rows and 12 columns.
- There are no missing values in the dataset.
- The target variable, "quality," ranges from 3 to 8.

## Feature Engineering

- Outliers were handled using log transformation.
- Multicolinearity was addressed by dropping the "density," "fixed acidity," and "pH" columns.

## Model Preparation

- The data was split into training and testing sets.
- Linear Regression was applied to predict wine quality.

## Model Evaluation

- The accuracy of the Linear Regression model was approximately 40%.
- Mean Absolute Error (MAE) was found to be 0.502.
- The Root Mean Squared Error (RMSE) was 0.71.

## Conclusion

This project aimed to predict wine quality using linear regression. While the model showed limited accuracy, it serves as a starting point for further improvement and exploration of more advanced techniques.

Feel free to fork and enhance this project to improve the predictive performance or explore other machine learning algorithms.

