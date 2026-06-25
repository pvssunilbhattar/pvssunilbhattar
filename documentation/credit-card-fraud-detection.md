# Credit Card Fraud Detection

## Project Overview

This project focuses on building a predictive machine learning solution for detecting fraudulent credit card transactions. The goal is to identify suspicious transactions quickly so that financial institutions and online merchants can reduce fraud losses, improve customer trust, and strengthen transaction security.

## Problem Statement

The rise of digital payments, online shopping, mobile banking, and electronic transactions has increased the risk of fraud. Credit card fraud is especially challenging because fraud patterns evolve quickly and require models that can detect suspicious behavior from transaction data in near real time.

## Target Users

- Banks and financial institutions
- Credit card companies
- Online merchants and e-commerce platforms
- Fraud prevention and risk analytics teams

## Dataset

The project used a credit card fraud transaction dataset sourced from Kaggle. The data included transaction-level information such as amount, card type, entry mode, transaction country, customer demographics, bank, merchant group, and fraud status.

## Data Cleaning and Preprocessing

Key preprocessing steps included:

- Removed unnecessary columns such as `Day of Week`
- Standardized date and time formats
- Merged date and time fields into a single timestamp column
- Renamed columns for clarity, such as `Shipping Address` to `Country of Shipping`
- Cleaned transaction IDs, amount values, and inconsistent bank names
- Converted age and amount fields into numeric data types
- Handled missing values using mode imputation or row removal where appropriate
- Treated age outliers using IQR-based capping
- Removed duplicate records
- Applied label encoding and one-hot encoding for categorical variables
- Normalized numerical columns using Min-Max scaling

## Exploratory Data Analysis

The project explored transaction patterns using visualizations and statistical summaries. EDA included:

- Transaction amount distribution
- Transaction distribution by gender
- Card type distribution between Visa and MasterCard
- Entry mode distribution across CVC, PIN, and Tap
- Fraud vs. non-fraud transaction distribution
- Fraud distribution by gender
- Fraud patterns by card type, country, bank, age, and transaction hour
- Correlation analysis between transaction attributes and fraud status

## Machine Learning Models

Multiple models were trained and compared:

- Logistic Regression
- Naive Bayes
- Support Vector Machine with RBF kernel
- K-Means Clustering
- Random Forest Classifier
- Gradient Boosting Machine
- Multi-Layer Perceptron

## Model Findings

Gradient Boosting Machine produced the strongest overall result with high accuracy and balanced precision-recall performance. Random Forest and SVM also performed strongly, while Naive Bayes showed high recall but lower precision, creating more false positives. K-Means performed weakest for supervised fraud detection because the problem required more reliable classification boundaries.

## Final Outcome

The project demonstrates an end-to-end fraud analytics workflow, starting from raw transaction data and progressing through data cleaning, EDA, feature engineering, modeling, evaluation, and final model comparison. The final recommendation favored Gradient Boosting Machine because of its ability to detect fraud accurately while maintaining a balanced trade-off between fraud recall and false-positive control.

## Skills Demonstrated

- Python
- Pandas and NumPy
- Scikit-learn
- Data cleaning and preprocessing
- Exploratory data analysis
- Feature engineering
- Classification modeling
- Model evaluation
- Fraud analytics
- Predictive modeling

## Portfolio Value

This project shows practical experience in financial fraud detection, model comparison, real-world classification challenges, and data-driven decision-making for risk analytics.