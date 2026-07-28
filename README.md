# HCUP Emergency Department Health Cost Prediction

## Overview

This project develops machine learning models to predict emergency department (ED) charges using the 2016 Healthcare Cost and Utilization Project (HCUP) Nationwide Emergency Department Sample (NEDS). The objective is to identify the factors that contribute most to healthcare costs and evaluate the performance of different regression algorithms on a large-scale healthcare dataset.

This work demonstrates the complete machine learning pipeline, including data preprocessing, feature engineering, model development, evaluation, and interpretation.

---

## Objectives

- Predict total emergency department charges (`TOTCHG_ED`)
- Analyze the impact of patient demographics, hospital characteristics, diagnoses, and payer information on healthcare costs
- Compare multiple machine learning regression algorithms
- Build an efficient pipeline capable of handling tens of millions of healthcare records

---

## Dataset

**Source:** HCUP Nationwide Emergency Department Sample (NEDS) 2016

- Approximately **32.7 million** emergency department visits
- **56 variables** describing patient, hospital, diagnosis, and billing information
- Dataset size: approximately **11 GB** after extraction

**Target Variable**

- `TOTCHG_ED` — Total Emergency Department Charges

> **Note:** The HCUP dataset is not included in this repository due to HCUP's Data Use Agreement.

---

## Data Preprocessing

The following preprocessing steps were performed:

- Removed unnecessary columns
- Handled missing values
- Encoded categorical variables
- Selected relevant predictive features
- Prepared data for machine learning models
- Split data into training and testing datasets

---

## Machine Learning Models

The following regression algorithms were implemented and compared:

- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor

Each model was trained using the same feature set and evaluated using identical performance metrics.

---

## Model Evaluation

Models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score (Coefficient of Determination)

The performance comparison helped identify the best model for predicting emergency department charges.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Jupyter Notebook

---

## Project Workflow

1. Load HCUP NEDS dataset
2. Clean and preprocess data
3. Engineer and select features
4. Split data into training and testing sets
5. Train multiple regression models
6. Evaluate model performance
7. Compare results and analyze feature importance


## Future Improvements

- Hyperparameter optimization
- Cross-validation
- SHAP explainability analysis
- Deep learning models
- Deployment as a prediction API

---

## Disclaimer

The HCUP NEDS dataset is proprietary and distributed under the HCUP Data Use Agreement. Therefore, the raw dataset is **not included** in this repository. Users must obtain access directly through HCUP before running this project.
