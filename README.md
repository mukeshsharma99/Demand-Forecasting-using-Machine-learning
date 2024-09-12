# Demand-Forecasting-using-Machine-learning
This project aims to predict the demand (sales) for various products sold in multiple stores across different time periods.

# Project Overview
This project aims to predict the demand (sales) for various products sold in multiple stores across different time periods. By leveraging historical sales data and applying advanced machine learning techniques, the project intends to forecast the stock requirements for products, helping businesses optimize their inventory and avoid overstocking or understocking situations.

The project includes various stages such as data preprocessing, feature engineering, exploratory data analysis (EDA), model training, evaluation, and deployment of the best-performing model.

# Table of Contents

- [Project Overview](#project-overview)
- [ Dataset](####train.csv)
- [Project Structure](####project-structure)
- [Problem Statement](####problem-statement)
- [Solution Approach](####solution-approach)
  - Data Preprocessing
  - Feature Engineering
  - Exploratory Data Analysis
  - Model Training
  - Model Evaluation
- [Technologies Used](####technologies-used)

  ## Dataset
The dataset consists of historical sales data for different products across multiple stores. The data spans several years, containing the following columns:

Date: The date of the sales record.
Store: The ID of the store.
Item: The ID of the product.
Sales: The number of items sold.

## Problem Statement
The goal of this project is to develop a machine learning model that can accurately forecast product demand across multiple stores based on historical data. The model must predict future sales while considering seasonality, trends, and other external factors (such as holidays and weekends).

Predicting future demand will help businesses plan their inventory effectively, reducing both stock shortages and excess stock.

## Solution Approach
#### 1. Data Preprocessing
Handling Date Column: The date column was split into year, month, and day.
Feature Extraction: Additional features like weekends and holidays were added to enhance the dataset.
Normalization: Features were scaled using StandardScaler to ensure fast convergence of machine learning algorithms.
#### 2. Feature Engineering
Feature engineering plays a crucial role in improving model performance:

Cyclical Features: Since the month is a cyclical feature, it was transformed using sine and cosine functions to capture periodic behavior.
Weekend and Holiday Effects: It was hypothesized that weekends and holidays would affect sales, so these features were added to the dataset.
#### 3. Exploratory Data Analysis (EDA)
EDA was performed to gain insights into the relationships between features and the target variable (sales):

Bar Plots: Visualizations were created to see the average sales across various features like year, month, store, and product.

Line Plots: Sales patterns over time (monthly, daily) were analyzed.

Correlation Heatmap: To identify potential multicollinearity among the features, a correlation heatmap was generated.

#### 4. Model Training
Various machine learning models were trained on the preprocessed data to predict product demand:

Linear Regression: A basic model for capturing linear relationships.

Lasso: A linear regression model with L1 regularization to prevent overfitting.

Ridge: A linear regression model with L2 regularization.
#### 5. Model Evaluation
Models were evaluated using the Mean Absolute Error (MAE) on both the training and validation datasets.MAE was chosen as the evaluation metric because it measures the average magnitude of errors in a set of predictions, without considering their direction.

#### Technologies Used
Python: The main programming language used for data analysis and machine learning.

Pandas: For data manipulation and analysis.

NumPy: For numerical operations.

Matplotlib & Seaborn: For data visualization and plotting.

Scikit-learn: For machine learning models and data preprocessing.

Jupyter Notebook: For code execution and documentation.

