# Insurance Data Analysis and Modeling

## Overview

This project provides an exploratory data analysis (EDA) and predictive modeling pipeline for an insurance dataset. It includes data preprocessing, handling outliers, encoding categorical variables, and training machine learning models to predict insurance charges.

## Table of Contents

1. [Dataset Overview](#dataset-overview)
2. [Preprocessing Steps](#preprocessing-steps)
   - Environment Setup
   - Data Exploration
   - Handling Missing Values
   - Outlier Detection and Treatment
   - Encoding Categorical Columns
3. [Model Building](#model-building)
4. [Results and Insights](#results-and-insights)
5. [Conclusion](#conclusion)

## Dataset Overview

The dataset contains the following features:

- age: Age of the insured
- sex: Gender of the insured
- bmi: Body Mass Index
- children: Number of dependent children
- smoker: Smoking status
- region: Residential area
- charges (target variable): Medical insurance costs

## Preprocessing Steps

### Environment Setup

The following libraries are required:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

### Data Exploration

- Read the dataset and explore its structure, including data types and unique values.
- Separate features into categorical and numerical columns.

### Handling Missing Values

- No missing values were found in the dataset.

### Outlier Detection and Treatment

- Numerical features (`age`, `bmi`, `charges`) were analyzed for outliers using box plots.
- Outliers were capped using the IQR method.

### Encoding Categorical Columns

- Categorical columns (`sex`, `smoker`, `region`) were encoded using one-hot encoding.

## Model Building

Three models were trained to predict `charges`:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor

The dataset was split into training and test sets (80% train, 20% test). Evaluation metrics included:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

## Results and Insights

The performance of the models was compared based on the test set. The Random Forest Regressor emerged as the best model with the lowest MAE and RMSE.

A scatter plot comparing actual and predicted charges for the best model was generated.

## Conclusion

This project demonstrates the complete workflow of data analysis and predictive modeling. The Random Forest Regressor is recommended for similar datasets due to its robustness and accuracy.
