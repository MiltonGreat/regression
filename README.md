# Canada Rent Regression Project

## Overview

This project involves analyzing rental prices for units across Canada in 2024 using regression models. The goal is to explore multiple regression models and find the one that predicts rental prices most accurately. The analysis includes exploratory data analysis (EDA), data cleaning and preparation, feature engineering, and comparison of regression models.

## Dataset

The dataset `canada_rent.csv` contains rental prices and associated features for units in Canada. 

## Project Steps:

1. Use canada_rent.csv dataset to predict rental prices in Canada for 2024
2. Perform Exploratory Data Analysis (EDA)
3. Clean and prepare the data
4. Use feature engineering where necessary
5. Compare at least 3 regression models
6. Choose a validation scheme
7. Explain feature selection for the final model
8. Use the final model to make new predictions

## Key Concepts Covered:

# 1. What are the key factors affecting rental prices in different regions of Canada for 2024?

- Latitude and Longitude
- Beds
- Baths
- Square Feet
- Price Per Square Foot
- Property Type (e.g., Storage, Townhouse, Vacation Home)
- Furnishing Status (e.g., Unfurnished, Negotiable)
- Smoking Policy (e.g., Non-Smoking, Smoke-Free Building, Smoking Allowed)

# 2. How accurate is the regression model in predicting rental prices compared to actual prices?

- Test Data - Mean Squared Error: 0.0140. The small size implies good model performance. 
- Test Data - Mean Absolute Error: 0.0260. This low value also implies good model perofmance.
- Test Data - R-squared: 0.9862. A very high value simplies a strong predictive power.

# 3. Which regression model provides the best balance between prediction accuracy and interpretability?

- I used Random Forest since my primary goal is to use a flexible model that can capture non-linear relationship.
- I had noticed problems with noise in the data set, so I chose Random Forest model over the simpler Lasso model. 
- In the end, the project compared the performance of Linear, Ridge, and Random Forest Regression.

# 4. What steps were taken to ensure that the model is not overfitting and generalizes well to unseen data?

- Train-Test Split
- Regularization
- Cross-validation
- Model Selection
- Hyperparameter Tuning
- Model Evaluation and Test Set
