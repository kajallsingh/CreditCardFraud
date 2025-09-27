
Credit Card Fraud Detection using Machine Learning

📖 Project Overview
This project detects fraudulent credit card transactions using machine learning models. The dataset is highly imbalanced, with only a small fraction of transactions being fraud. The project demonstrates data preprocessing, model training, evaluation, and prediction of new transactions.

📊 Dataset
Source: Public credit card transactions dataset from kaggle

Features:
V1 to V28 — anonymized transaction features from PCA transformation
Amount — transaction amount
Class — target variable (0 = Not Fraud, 1 = Fraud)
Number of samples: 284,807 transactions
Imbalance: Only 492 fraud cases (~0.17% of total)

⚙️ Project Workflow
1. Data Preprocessing
Checked for missing values and handled them (none in this dataset).
Separated features (X) and target (y).
Split dataset into training and testing sets using stratified split to maintain class ratio.

2. Model Training
Trained multiple models:
Random Forest (with hyperparameter tuning using RandomizedSearchCV)
Gradient Boosting
XGBoost
LightGBM

3. Model Evaluation
Metrics used: Accuracy, Precision, Recall, F1-score
Confusion Matrix
ROC Curve & AUC
Feature Importance visualization

📈 Results
Confusion Matrix shows the number of correctly classified fraud and non-fraud transactions.
ROC Curve demonstrates trade-off between True Positive Rate and False Positive Rate.
Feature Importance shows which transaction features are most influential in predicting fraud.

🚀 Tech Stack
Python 

Data Analysis & Manipulation: 
pandas
NumPy  

Machine Learning: 
scikit-learn 
XGBoost 
LightGBM 

Data Visualization: 
matplotlib 
seaborn 

Model Saving: 
joblib 
