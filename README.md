# Stock Price Prediction with Machine Learning

## Overview

This project uses machine learning techniques to predict stock price movements based on historical data. The implemented models include Logistic Regression, Support Vector Machine (SVM), and XGBoost. The dataset used is from Amazon (AMZN) stock, and the goal is to predict whether the stock price will increase or decrease.

## Prerequisites

Before running the code, make sure you have the necessary libraries installed. You can install them using the following command:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
```

## Data

The dataset is loaded from a CSV file containing historical stock data of Amazon (AMZN). The file path can be customized as needed it was extracted via Yahoo Finance.

## Exploratory Data Analysis (EDA)

- The dataset is explored through various visualizations, including line plots, distribution plots, and box plots.
- Date features are extracted from the 'Date' column, and additional features like quarter-end indicators are created.

## Feature Engineering

- New features such as 'open-close' and 'low-high' are generated based on existing columns.
- A binary target variable is created to indicate whether the stock price will increase (1) or decrease (0) on the next day.

## Model Training

- StandardScaler is applied to scale the features.
- The dataset is split into training and validation sets.
- Logistic Regression, Support Vector Machine (SVM), and XGBoost models are trained and evaluated.

## Evaluation

- The models are evaluated using ROC AUC score on both the training and validation sets.
- Confusion matrices are visualized using seaborn heatmap for Logistic Regression.
- Having said that due to the oversimplfication of the model as well as the limitation of data, this model is not effective

## Acknowledgments

- Special thanks to the developers of scikit-learn, XGBoost, and other libraries used in this project.

