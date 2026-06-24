## AI/ML Engineering Internship Tasks - DevelopersHub Corporation

This repository contains the projects and tasks completed during my AI/ML Engineering Internship at DevelopersHub Corporation.

## Task 1: Exploring and Visualizing a Simple Dataset

### 1. Task Objective
The objective of this task is to load, inspect, and analyze the distributions, trends, and potential outliers within a basic dataset.

### 2. Dataset Used
Dataset Name: Iris Dataset (loaded natively via the Seaborn library).
Data Features: Sepal Length, Sepal Width, Petal Length, Petal Width, and Species classification.

### 3. Models Applied
Type of Analysis: Exploratory Data Analysis (EDA) and Statistical Visualization. No machine learning models were applied to this data tracking task.

### 4. Key Results and Findings
Species Distinctness:The `setosa` species is heavily separated from `versicolor` and `virginica` across all feature pairings in the scatter plot matrix.
Outlier Detection: The generated Box Plots successfully highlighted minor statistical data outliers present inside the `sepal_width` feature column.
Feature Ranges: Histograms revealed that petal dimensions display distinct gaps in value distributions compared to more uniform sepal measurements.

---

## Task 2: Predict Future Stock Prices (Short-Term)

### 1. Task Objective
The objective of this task is to fetch historical stock market data, pre-process it for time-series forecasting, and build a machine learning model to predict the next day's closing price.

### 2. Dataset Used
* **Source:** Yahoo Finance API (retrieved natively via the `yfinance` library).
* **Ticker analyzed:** AAPL (Apple Inc.).
* **Features Used:** Open, High, Low, and Volume to predict the target variable (`Next_Close`).

### 3. Models Applied
* **Algorithm:** Linear Regression (`scikit-learn`).
* **Data Split:** 80% Training, 20% Testing (Chronological sequential split without shuffling to preserve time-series order).

### 4. Key Results and Findings
* **Model Fit:** The trained Linear Regression model closely tracks real-market directional trends, matching actual closing shifts with minimal error.
* **Evaluation:** Evaluated performance metrics using Mean Absolute Error (MAE) and R-squared ($R^2$) to verify statistical accuracy before final model deployment.
