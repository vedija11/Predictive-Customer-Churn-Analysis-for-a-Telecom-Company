# Predictive Customer Churn Analysis for a Telecom Company

## Project Overview

This project analyzes customer churn for a telecom company and builds predictive models to identify at-risk customers. Using machine learning and data mining techniques, the goal is to enhance retention strategies and reduce revenue loss.

## Table of Contents

* [Project Overview](#project-overview)
* [Data](#data)
* [Exploratory Data Analysis](#exploratory-data-analysis)
* [Feature Selection & Engineering](#feature-selection--engineering)
* [Modeling](#modeling)
* [Model Evaluation](#model-evaluation)
* [Deployment & Recommendations](#deployment--recommendations)
* [Technologies Used](#technologies-used)
* [Future Work](#future-work)

## Data

* Customer demographic information, account details, and service usage patterns.
* Preprocessed to handle missing values, outliers, and categorical encoding for modeling.
* Split into training and test datasets for model development and validation.

## Exploratory Data Analysis

* Visualized churn distribution and explored patterns across contract types.
* Created correlation heatmaps for numerical features like Monthly Charges, Tenure, and Total Charges.
* Identified key patterns that influence customer retention.

## Feature Selection & Engineering

* Used Random Forest to rank feature importance.
* Top features: TotalCharges, Tenure, MonthlyCharges, and service-related variables.
* Removed less impactful variables to optimize model performance.

## Modeling

* **Logistic Regression**: Baseline model.
* **Decision Tree**: Captures nonlinear patterns.
* **Random Forest**: Ensemble model for reduced variance.
* **Support Vector Machine (SVM)**: Complex decision boundaries.
* **Gradient Boosting (GBM)**: Best-performing model with cross-validation.

## Model Evaluation

| Model                   | Accuracy | ROC AUC |
| ----------------------- | -------- | ------- |
| Logistic Regression     | 0.819    | 0.840   |
| Decision Tree           | 0.822    | 0.775   |
| Random Forest           | 0.814    | 0.808   |
| SVM                     | 0.818    | 0.753   |
| Gradient Boosting (GBM) | 0.821    | 0.846   |

* **Gradient Boosting** selected for deployment due to highest ROC AUC.

## Deployment & Recommendations

* Deployed model for real-time churn prediction.
* Recommendations:

  1. Personalized retention offers for high-risk customers.
  2. Service optimization for key features influencing churn.
  3. Loyalty programs to retain long-term customers.
  4. Early intervention strategies using predictive insights.

## Technologies Used

* Python, Pandas, Scikit-learn, Matplotlib, Seaborn, SQL, Gradient Boosting
