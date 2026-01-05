# Credit-Card-Fraud-Detection
Predicting whether a credit card transaction is fraudulent or legitimate.

## Project Overview

Credit card fraud detection is a binary classification problem aimed at identifying fraudulent transactions while minimizing false alerts for genuine customers.
This project builds and evaluates machine learning models on a highly imbalanced dataset, focusing on recall-driven fraud detection.

## Business Objective

* Detect fraudulent transactions early

* Minimize financial loss

* Reduce false declines for legitimate users

## Machine Learning Objective

* Classify transactions as Fraud (1) or Non-Fraud (0)

* Prioritize Recall over accuracy due to class imbalance

* Provide probability-based risk scoring for transaction review

## Dataset

Source: Kaggle

Dataset: Credit Card Fraud Detection (European Cardholders)

## Dataset Characteristics
* Attribute	Details
  
* Total Transactions	284,807
  
* Fraud Cases	492 (≈0.17%)
  
* Features	V1–V28 (PCA transformed)
  
* Target	Class (0 = Legit, 1 = Fraud)

## Key Challenge

* Class Imbalance

* Fraud transactions are extremely rare

* Accuracy is misleading

* Evaluation must focus on Recall, Precision, F1-Score, ROC-AUC

## Tech Stack

* Python

* Pandas, NumPy

* Scikit-learn

* Imbalanced-learn (SMOTE)

## Project Workflow

* Data Understanding & EDA

* Analyze class distribution

* Understand transaction amounts and fraud patterns

## Data Preprocessing

* Scale Amount and Time

* PCA features already standardized

* Stratified train-test split

## Handling Class Imbalance

* Applied SMOTE (Synthetic Minority Over-sampling Technique)

* Compared with class-weighted models

## Model Building

* Logistic Regression (Baseline)

* Random Forest Classifier

* XGBoost Classifier

## Model Evaluation

Metrics used:

* Recall

* Precision

* F1-Score

* ROC-AUC

 * Recall was prioritized to avoid missing fraudulent transactions.

 * Fraud Probability Scoring

## Instead of only binary prediction:

* Generated fraud probability scores

* Tuned decision threshold (lower than 0.5)

* Flagged high-risk transactions for review

## Sample Output
  
 Fraud_Probability	Predicted_Class	Actual_Class
0.96	1	1
0.89	1	0
0.75	1	1
  
## Results

* Improved fraud detection recall significantly

* Balanced precision to reduce false alarms

* Enabled risk-based transaction monitoring

## Future Improvements

* Cost-sensitive learning

* Real-time fraud detection pipeline

* Anomaly detection using Isolation Forest

## Conclusion

This project demonstrates a real-world machine learning solution for fraud detection, emphasizing imbalanced data handling, probability-based predictions, and business-oriented evaluation metrics.

<img width="397" height="383" alt="Screenshot 2026-01-05 173842" src="https://github.com/user-attachments/assets/188408c7-0474-43dd-b9b4-17f46ead5f79" />

