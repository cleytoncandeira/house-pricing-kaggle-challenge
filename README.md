# House Price Prediction Challenge on Kaggle


![House Price Prediction Challenge](https://miro.medium.com/v2/resize:fit:760/1*_wu6ec7zO54fqqEk0lzrmw.jpeg)


## Overview

This repository contains my solution to the House Price Prediction challenge on Kaggle. The goal of this challenge is to predict the sale prices of houses based on a set of features. In this README, I'll provide an overview of the key steps and techniques I used to tackle this challenge.

## Feature Engineering
### Ordinal Variables

I started by working with ordinal variables. To handle these, I created a dictionary that mapped the ordinal levels to numerical values. I further improved this dictionary to ensure that the numerical values accurately represented the order of the levels.
Numeric Variables

I applied various transformations to the numeric variables to make them more suitable for modeling. These transformations included Box-Cox transformations, logarithmic transformations, and square root transformations to normalize the data and improve its distribution.
Handling Missing Data

I used decision tree-based classifiers to predict and fill missing values in categorical variables such as 'MSZoning.' This helped in preserving the integrity of the dataset.

## Exploratory Data Analysis (EDA)
### Variable Relationships

To understand the relationships between variables, I employed statistical techniques such as Pearson correlation, chi-squared test, and Cramer's V criterion. These analyses helped identify key correlations and associations within the dataset.
Multicollinearity

To address multicollinearity issues among variables, I created indicator variables such as 'Renovated,' 'FullBathDensity,' and 'BAFFAreaRatio.' These indicators helped mitigate multicollinearity concerns and improve model stability.

## Model Selection

I implemented a function to choose the best regression model for this task. I evaluated various models, including:

    Ridge Regression
    Lasso Regression
    Artificial Neural Network (ANN)
    XGBoost
    Gradient Boosting
    Random Forest
    Support Vector Regression (SVR)
    ElasticNet

The evaluation involved assessing each model's performance based on relevant metrics and selecting the one that yielded the best results for this specific prediction task.
