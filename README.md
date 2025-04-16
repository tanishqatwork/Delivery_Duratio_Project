# Delivery Duration Prediction

This repository contains an end-to-end data science project focused on predicting the delivery duration of food orders. The project is based on a dataset from StrataScratch and follows a structured approach from data exploration and feature engineering to model building and evaluation using both classical machine learning and deep learning techniques.

## Table of Contents

- [Assignment](#assignment)
- [Data Exploration](#data-exploration)
- [Feature Engineering](#feature-engineering)
  - [Multicollinearity Check](#multicollinearity-check)
  - [Feature Selection](#feature-selection)
- [Scaling and Inverse Transformation](#scaling-and-inverse-transformation)
- [Classical Machine Learning Models](#classical-machine-learning-models)
- [Deep Learning Approach](#deep-learning-approach)
- [Results and Observations](#results-and-observations)
- [How to Use](#how-to-use)
- [Contributors](#contributors)
- [License](#license)

---

## Assignment

The goal of this project is to accurately predict the total delivery duration from the time an order is placed until it is delivered. This project leverages a variety of features and uses data sourced from [Kaggle – DoorDash ETA Prediction Dataset](https://www.kaggle.com/datasets/dharun4772/doordash-eta-prediction).

---

## Data Exploration

In this section, the dataset is thoroughly analyzed to understand its structure, check for missing values, and perform initial visualizations to capture key relationships between features. The exploration sets the foundation for subsequent feature engineering and model training.

---

## Feature Engineering

### Multicollinearity Check
We analyze feature correlations to detect and mitigate multicollinearity. Removing or combining highly correlated features helps improve model robustness.

### Feature Selection
Using techniques such as feature importance from tree-based models and univariate statistical tests, key features are selected. For example, the project uses a sorted list of features based on a "Gini-importance" measure (filtered to include only columns present in the data) to build models.

---

## Scaling and Inverse Transformation

The dataset undergoes scaling (using `StandardScaler` in our primary approach) to ensure features contribute equally to model training. An inverse transformation is applied later so that predicted values and error metrics (like RMSE) can be interpreted on the original scale.

---

## Classical Machine Learning Models

Several regression models are trained and evaluated in this project, including:

- **Linear Regression**
- **Ridge Regression**
- **Decision Trees**
- **Random Forests**
- **XGBoost**
- **LightGBM**
- **MLP Regressor**

For each model, the training process, prediction, and error metric computations (e.g., RMSE) are performed. A custom function (`make_regression`) is used to streamline model fitting and prediction.

---

## Deep Learning Approach

In addition to traditional models, a deep learning approach is explored. This section includes details about network architecture, training procedures, and comparative performance analysis with classical methods.

---

## Results and Observations

A comparative analysis is provided for all models. The key insights include:
- Which features most significantly impact delivery duration.
- The best performing models in terms of accuracy.
- Observations on the impact of data scaling and inverse transformations on error metrics.


