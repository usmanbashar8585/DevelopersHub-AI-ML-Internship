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
* ---

## Task 3: Heart Disease Prediction (Binary Classification)

### 1. Task Objective
The objective of this task is to build a machine learning classification system capable of analyzing clinical patient health metrics and predicting whether a individual is at risk of heart disease.

### 2. Dataset Used
* **Source:** Heart Disease UCI Dataset (retrieved via an online CSV mirror).
* **Target Variable:** `target` (0 = Healthy / No Risk, 1 = Heart Disease Risk).
* **Clinical Features Analyzed:** Age, Sex, Chest Pain Type (`cp`), Resting Blood Pressure (`trestbps`), Serum Cholesterol (`chol`), Fasting Blood Sugar (`fbs`), Resting Electrocardiographic Results (`restecg`), Maximum Heart Rate Achieved (`thalach`), Exercise Induced Angina (`exang`), ST depression (`oldpeak`), Slope, Number of Major Vessels (`ca`), and Thal.

### 3. Models Applied
* **Algorithm:** Logistic Regression (`scikit-learn`), scaled to 1000 iterations to ensure full gradient convergence.
* **Data Split:** Stratified 80% Training and 20% Testing split to maintain an equal ratio of healthy vs risk cases across both datasets.

### 4. Key Results and Findings
* **Model Accuracy:** Successfully trained the classifier to separate healthy individuals from risk cases with high overall prediction accuracy.
* **Error Diagnosis:** Evaluated model errors using a visual Confusion Matrix to measure false positives and false negatives.
* **ROC-AUC Performance:** Generated a Receiver Operating Characteristic (ROC) curve to confirm structural precision and strong target class separation.
* **Feature Importance:** Coefficient analysis highlighted attributes like chest pain types (`cp`) and maximum heart rate (`thalach`) as top positive indicators contributing to cardiac risk prediction.
