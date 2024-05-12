# Project Name

## Overview

[Provide a brief overview of your project here.]

## Handling Outliers

### **Handling Outlier**

Recognizing and addressing data points that significantly depart from the bulk of the collection constitutes handling outliers. In our situation, 184 unexpected negative results that may be a sign of problems with data quality were found after carefully examining the training set. We chose to eliminate these negative values in order to preserve the integrity of the training data and avoid any potential biases in statistical analysis or machine learning model training. We then looked over the testing dataset and discovered that there were no negative values, confirming the testing data's dependability and consistency. The robustness and validity of our data analysis and modeling efforts are guaranteed by this methodical approach to handle outliers.

## Model Selection

### **We chose LightGBM model for prediction**

We chose the LightGBM model for prediction because we observed that its MSE (Mean Squared Error) value is lower compared to the other three models. This indicates that LightGBM provides better accuracy in predicting the target variable based on our dataset.

## My Approach

**My approach involved simple preprocessing. I used label encoding only for the product size because it contains levels like small, large, extra-large, etc. For the remaining features, I applied one-hot encoding. To handle the 'Month of Sourcing' column, I first converted it to a datetime object, and then to an integer. That sums up my approach to data cleaning.**


