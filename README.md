# Loan Default Prediction & Analysis

A machine learning and exploratory data analysis project focused on identifying factors associated with loan repayment difficulties and predicting whether a client is likely to repay a loan.

## Overview

The project analyzes two datasets — `application_data` and `previous_application` — containing information about loan applicants, their financial characteristics, previous applications, and loan outcomes. The goal is to understand patterns associated with loan defaults and build models that can predict repayment outcomes.

## Approach

The project follows an end-to-end data analysis and machine learning workflow:

1. Imported and explored application and previous-application datasets.
2. Analyzed missing values and handled missing numerical and categorical data.
3. Identified and addressed columns with excessive missing values.
4. Detected and capped outliers in numerical variables.
5. Encoded categorical variables and prepared numerical features.
6. Performed univariate and bivariate analysis to identify patterns associated with loan defaults.
7. Merged application and previous-application data for further analysis.
8. Built machine learning pipelines for repayment prediction.
9. Used Decision Tree models to predict repayment outcomes and annuity amounts.
10. Generated repayment labels such as `Will repay` and `Will not repay`.

## Machine Learning

Two Decision Tree models were developed:

- **Decision Tree Classifier** — predicts whether a client is likely to experience difficulty repaying the loan.
- **Decision Tree Regressor** — predicts the loan annuity amount.

The models use preprocessing pipelines with median imputation for numerical features and one-hot encoding for categorical features.

## Key Findings

The exploratory analysis identified several patterns associated with higher default rates, including unemployment, maternity leave, lower-secondary education, younger applicants, and certain loan and housing characteristics.

The analysis also found that the dataset was highly imbalanced, with approximately **91.9% of applications belonging to clients without repayment difficulties and 8.1% representing repayment difficulties**.

## Technologies & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

## Dataset

The project uses the **Home Credit** application and previous-application datasets.

The raw datasets are not included in this repository.

## Project Structure

```text
loan-default-prediction/
│
├── Fraud_Detection_System.ipynb
├── README.md
└── requirements.txt
