# Fraud Detection Model - README

## Overview
This project implements a machine learning model to detect fraudulent financial transactions. The dataset consists of **6,362,620 financial transactions** with **11 features**, including transaction type, amount, origin/destination accounts, balances, and fraud indicators. Only **0.13% of transactions (8,211 cases)** are fraudulent, with fraud primarily occurring in **TRANSFER** and **CASH_OUT** transactions.

## Project Structure
The notebook follows a structured approach to fraud detection:

1. **Environment Setup and Data Loading**
2. **Exploratory Data Analysis (EDA)**
3. **Data Preprocessing and Feature Engineering**
4. **Feature Selection**
5. **Data Splitting and Resampling**
6. **Initial Model Training for Feature Selection**
7. **Final Model Training**
8. **Model Evaluation**
9. **Model Interpretation**
10. **Fraud Pattern Analysis**
11. **Threshold Optimization**
12. **Model Deployment Preparation**
13. **Key Insights**
14. **Final Summary**

## Key Findings
- **Fraud Distribution**: Only 0.13% of transactions are fraudulent, making this a highly imbalanced classification problem.
- **Transaction Types**: Fraud occurs mainly in TRANSFER and CASH_OUT transactions.
- **Amount Analysis**: High-value transactions are more susceptible to fraud.
- **Feature Importance**: The model identifies key features that are most predictive of fraudulent activity.

## Dependencies
- Python 3.10.12
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost
- imblearn

## Usage
1. Clone the repository
2. Install required dependencies: `pip install -r requirements.txt`
3. Run the Jupyter notebook: `jupyter notebook Fraud-detection.ipynb`

## Data
The dataset is sourced from Kaggle and contains the following features:
- `step`: timestamp (in hours)
- `type`: transaction type (PAYMENT, TRANSFER, CASH_OUT, etc.)
- `amount`: transaction amount
- `nameOrig`: origin account
- `oldbalanceOrg`: origin balance before transaction
- `newbalanceOrig`: origin balance after transaction
- `nameDest`: destination account
- `oldbalanceDest`: destination balance before transaction
- `newbalanceDest`: destination balance after transaction
- `isFraud`: fraud indicator (target variable)
- `isFlaggedFraud`: flagged fraud indicator

## Model Performance
The notebook includes detailed evaluation metrics including:
- Classification report
- Confusion matrix
- ROC curve and AUC
- Precision-recall curve

## How to Contribute
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

## License
This project is licensed under the MIT License.
