# Customer-Behaviour-Analysis
Purpose: Customer Behaviour Analytics for strategic business optimization

## Project Overview
This repository contains a comprehensive analysis of customer behavior to uncover insights that drive business decisions. 
The analysis includes exploratory data analysis (EDA), correlation analysis, class imbalance handling, 
and predictive modeling to identify purchase patterns and spending behaviors.

## Dataset Overview
- Number of Records: 50,000
- Features: 16 columns
- Target Columns: Will_Purchase, Annual_Spending

## Key Analyses Performed
1. Exploratory Data Analysis (EDA)
    - Univariate Analysis: Distribution, skewness, and feature counts.
        - Income distribution peaked around middle.
        - Majority of customers have low online activity (right-skewed).
    - Bivariate Analysis: Relationships and dependencies between features.
        - Strong positive correlation between Online Activity Level and Online Purchase Tendency.
        - Loyal customers tend to spend more annually.

2. Class Imbalance Handling
    - Will_Purchase is highly imbalanced (majority of customers do not purchase).
        - Applied:
            - Oversampling (SMOTE) to increase minority class.
            - Downsampling to reduce majority class.

3. Correlation Analysis
    - Strong Positive Correlations Identified:
        - Online Activity Level & Online Purchase Tendency
        - Customer Loyalty Score & Annual Spending
        - Purchases in Last Month & Online Purchase Tendency

4. Predictive Modeling
    - Target 1: Will_Purchase (Classification)
        - Models: Random Forest, XGBoost
        - Evaluation: Accuracy, F1-score, ROC-AUC
    - Target 2: Annual_Spending (Regression)
        - Models: Random Forest Regressor, XGBoost Regressor
        - Evaluation: RMSE, R-squared

## Key Insights Discovered
- Loyalty scores, recent purchases, and discounts are the strongest purchase drivers.
- High-income customers do not always have high spending—behavior patterns are more predictive than demographics.
- Online activity alone is not a reliable predictor of purchases without considering loyalty and recent behavior.
- Online Purchase Tendency & Online Activity Level: customers who are more active online are also more likely to make purchase.
- Customer Loyalty Score & Annual Spending: loyal customers tend to spend more money annually.
- Online Purchase Tendency & Purchases in Last Month: customers who made purchases in the last month are more likely to purchase online in the future.
