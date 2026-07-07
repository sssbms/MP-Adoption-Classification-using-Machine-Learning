# MP-Adoption-Classification-using-Machine-Learning

## Project Overview

This project aims to identify GO+ users who are most likely to adopt MP Investment products using machine learning.

The analysis focuses on customers who:

- Do not have UT accounts, Agency Accounts, or IUTA registration
- Have average GO+ AUM ≥ RM5,000 or Total Cash In ≥ RM5,000
- Reside in Selangor or Kuala Lumpur

## Data Used

Customer information includes:

- Age
- Race
- State
- Annual Income
- Average GO+ AUM
- Cash In / Cash Out Amount
- Cash In / Cash Out Count
- Education Level
- Current MP Investment Status

## Methodology

### Feature Engineering

Additional features were created, including:

- Cash In Average
- Cash Out Average
- Cash Intensity (Cash In – Cash Out)
- High Activity Indicator

### Models Evaluated

- XGBoost
- Decision Tree
- Random Forest
- LightGBM

### Model Tuning

- Optuna Hyperparameter Optimization
- SMOTE Comparison
- Feature Importance Analysis
- Decision Tree Visualization

## Key Findings

The strongest predictors of MP Investment adoption were:

1. Average GO+ AUM
2. Age
3. Annual Income
4. Cash Intensity
5. Cash In Count

Decision Tree segmentation was used to identify customer groups with a high probability of MP adoption.

## High-Probability Segments

Using a minimum adoption probability threshold of **70%**, several high-potential customer groups were identified, including:

- Young customers (< 25 years old) with high AUM balances
- Customers with income above RM60,000 and AUM above RM2,000
- Customers with AUM above RM11,000 and strong GO+ activity
- Affluent customers (income > RM250,000)
- Older customers with AUM above RM20,000

The largest high-potential segment consisted of customers:

- Income > RM60,000
- AUM > RM11,619
- Age < 47

with an estimated **72.2% probability** of investing in MP.

## Tools & Libraries

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- LightGBM
- Optuna
- Imbalanced-Learn (SMOTE)
- Matplotlib

## Business Impact

The model provides an explainable framework for identifying GO+ customers who are most likely to adopt MP Investment products, enabling more targeted and efficient marketing campaigns.
