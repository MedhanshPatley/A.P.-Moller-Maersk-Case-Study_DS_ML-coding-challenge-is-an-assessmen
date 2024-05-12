# A.P.-Moller-Maersk-Case-Study_DS_ML

## Overview

In this project, we utilized an 11-month training dataset containing the following columns: ProductType, Manufacturer, Area Code, Sourcing Channel, Product Size, Product Type, Month of Sourcing, and Sourcing Cost. Our goal was to predict the sourcing cost for June 2021.


## Handling Outliers

### **Handling Outlier**

Recognizing and addressing data points that significantly depart from the bulk of the collection constitutes handling outliers. In our situation, 184 unexpected negative results that may be a sign of problems with data quality were found after carefully examining the training set. We chose to eliminate these negative values in order to preserve the integrity of the training data and avoid any potential biases in statistical analysis or machine learning model training. We then looked over the testing dataset and discovered that there were no negative values, confirming the testing data's dependability and consistency. The robustness and validity of our data analysis and modeling efforts are guaranteed by this methodical approach to handle outliers.

## Model Selection

### **We chose LightGBM model for prediction**

We chose the LightGBM model for prediction because we observed that its MSE (Mean Squared Error) value is lower compared to the other four models. This indicates that LightGBM provides better accuracy in predicting the target variable based on our dataset.

## My Approach

**My approach involved simple preprocessing. I used label encoding only for the product size because it contains levels like small, large, extra-large, etc. For the remaining features, I applied one-hot encoding. To handle the 'Month of Sourcing' column, I first converted it to a datetime object, and then to an integer. That sums up my approach to data cleaning.**

# Metrics

| Metrics          | RandomForestRegressor | LigthGBM | XGBOOST | DesicionTreeRegressor | GradientBoostingRegressor |
|------------------|----------------------|--------|-------|----------------------|-------------------------|
| Mse              | 1091.12              | 672.6  | 1038.98| 1093.9               | 1219.9                  |
| Mae              | 16.5                 | 18.4   | 19.13 | 16.6                 | 23.21                   |

