# Car Price Prediction Using Machine Learning

## Overview

This project focuses on predicting used car prices using machine learning techniques. The objective is to build a regression model that can estimate the market price of a vehicle based on its specifications, technical features, and seller information.

The project follows a complete machine learning workflow including data exploration, preprocessing, model training, hyperparameter tuning, and performance evaluation.

---

## Dataset

The dataset contains information about approximately 8,000 used vehicles and includes features such as:

* Brand
* Model
* Trim
* Body Type
* Fuel Type
* Transmission Type
* Engine Capacity
* Horsepower
* Exterior Color
* Interior Color
* Warranty Status
* City
* Seller Type

### Target Variable

* Price

---

## Exploratory Data Analysis (EDA)

Several visualizations were created to understand the dataset:

* Distribution of car prices
* Average price by brand
* Horsepower vs. price relationship
* Missing value analysis
* Statistical summaries

These analyses helped identify important patterns and prepare the data for modeling.

---

## Data Preprocessing

The following preprocessing steps were applied:

### Numerical Features

* Missing values replaced using median imputation
* Standardization using StandardScaler

### Categorical Features

* Missing values replaced using the most frequent category
* One-Hot Encoding applied using OneHotEncoder

### Additional Processing

* Converted engine capacity and horsepower ranges into numeric average values
* Combined preprocessing steps using ColumnTransformer and Pipeline

---

## Machine Learning Models

Three regression models were trained and compared:

### 1. Ridge Regression

A regularized linear regression model used as a baseline.

### 2. K-Nearest Neighbors (KNN) Regression

A distance-based regression model that predicts prices using similar vehicles.

### 3. Random Forest Regressor

An ensemble learning model based on multiple decision trees.

Hyperparameter tuning was performed using:

* GridSearchCV
* RandomizedSearchCV

to find the best-performing model configuration.

---

## Model Evaluation

The models were evaluated using:

* R² Score
* Mean Squared Error (MSE)

Performance was measured on both training and testing datasets to assess model generalization and detect overfitting.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Project Structure

```text
├── car_data.csv
├── Car Price Prediction.ipynb
├── README.md
```

---

## Key Learning Outcomes

Through this project I gained practical experience in:

* Data preprocessing
* Feature engineering
* Exploratory Data Analysis (EDA)
* Machine Learning Pipelines
* Hyperparameter Optimization
* Regression Modeling
* Model Evaluation and Comparison

---

## Future Improvements

* Add more vehicle-related features
* Test Gradient Boosting and XGBoost models
* Deploy the model as a web application
* Implement automated prediction APIs
* Improve feature engineering techniques

---

## Author

**Md Sifat Hossen**

Bachelor of Data Science Student

This project was completed as part of a university Hands-on Machine Learning and Data Science coursework project. It demonstrates the application of data preprocessing, exploratory data analysis, feature engineering, machine learning model development, hyperparameter tuning, and model evaluation techniques on a real-world used car price prediction problem.
