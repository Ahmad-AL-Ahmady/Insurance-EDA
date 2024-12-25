# Insurance Cost Prediction Project

## Overview

This project analyzes an insurance dataset to predict medical charges based on various personal attributes. The project includes comprehensive data preprocessing, exploratory data analysis (EDA), and the implementation of multiple regression models to predict insurance costs.

## Dataset

The dataset contains the following features:

- age: Age of the insured
- sex: Gender of the insured
- bmi: Body Mass Index
- children: Number of dependent children
- smoker: Smoking status
- region: Residential area
- charges (target variable): Medical insurance costs

## Project Structure

The project is organized into two main sections:

### 1. Data Preprocessing

- Dataset loading and initial exploration
- Data type conversion and categorical analysis
- Missing value detection and handling
- Outlier detection and treatment using IQR method
- Duplicate record checking
- Low variance feature analysis
- Feature encoding (One-Hot Encoding for categorical variables)

### 2. Model Building

- Train-test split (80-20)
- Implementation of four regression models:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - XGBoost Regressor
- Model evaluation using multiple metrics:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score (Coefficient of Determination)

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost

## Key Findings

- No missing values in the dataset
- Outliers present in 'charges' and 'bmi' columns
- No rare categories in categorical variables
- No duplicate records
- All features showed sufficient variance (no low-variance columns dropped)
- [Best performing model] achieved the highest R² score of [score]
- Feature importance analysis revealed [top features] as the most significant predictors

## Visualization

The project includes various visualizations:

- Box plots for outlier detection
- Distribution plots for numerical features
- Actual vs Predicted charges plot for model evaluation
- Feature importance plots for tree-based models

## Model Performance

Comparison of models based on:

- Training and Test MAE
- Training and Test RMSE
- Training and Test R² scores
- Feature importance analysis for each model

## Future Improvements

- Hyperparameter tuning for all models
- Implementation of additional advanced models
- Cross-validation for more robust model evaluation
- Feature engineering to create new meaningful features
- Ensemble methods combining multiple models

## Usage

1. Install required packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

2. Load the insurance dataset

3. Run the notebook sequentially to reproduce the analysis
