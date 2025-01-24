# Sales-Forecasting

This repository contains a project focused on forecasting sales using time series analysis and machine learning techniques. The project demonstrates preprocessing, feature engineering, and model training to predict monthly sales.

# Features

Data preprocessing: Cleaning and transforming sales data.
Exploratory Data Analysis (EDA): Visualizing sales trends.
Feature engineering: Creating supervised learning features.
Model training: Implementing machine learning models like Linear Regression.
Performance evaluation: Calculating metrics (MSE, MAE, R²).

Dependencies:
Ensure you have the following Python libraries installed:
os
pandas
numpy
matplotlib
seaborn
xgboost
sklearn
tensorflow

# Dataset

The dataset used in this project is an Excel file named Sales Data.xlsx. It contains the following columns:
date: Timestamp of sales.
store: Store identifier (removed during preprocessing).
item: Item identifier (removed during preprocessing).
sales: Monthly sales values.

Code Overview

1. Data Loading and Cleaning
Load the dataset using pandas.
Drop unnecessary columns (store, item).
Convert date to monthly periods and aggregate sales data.

2. Exploratory Data Analysis
Visualize monthly sales trends using matplotlib.

3. Feature Engineering
Compute sales differences (sales_diff) to remove trends.
Create lag features for supervised learning.

4. Data Splitting and Scaling
Split data into training and testing sets (last 12 months as test data).
Scale features using MinMaxScaler to normalize values between -1 and 1.

5. Model Training and Prediction
Linear Regression
Train a LinearRegression model.
Generate predictions and inverse-transform results.
Calculate evaluation metrics:
Mean Squared Error (MSE)
Mean Absolute Error (MAE)
R-squared (R²)

6. Visualization
Plot actual vs. predicted sales for visual comparison.

The trained model predicts monthly sales effectively, with metrics:

MSE: [16221.272385416869]
MAE: [12433.184266490736]
R²: [0.9906152516380969]
