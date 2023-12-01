# Financial_Fraud_Detection_model
# Fraud Detection in Financial Transactions

## Overview
This project aims to detect and prevent fraud in financial transactions using machine learning techniques. The implemented model analyzes transaction patterns, identifies anomalies, and triggers alerts for suspicious activity.

## Dataset
The dataset used in this project is loaded from a CSV file (`credit_data.csv`). It contains information about credit card transactions, with two classes: 0 for normal transactions and 1 for fraudulent transactions. The dataset is highly unbalanced, with significantly more normal transactions than fraudulent ones.

### Dataset Information
- Loaded using Pandas DataFrame
- Checked for missing values
- Explored the distribution of legitimate and fraudulent transactions

## Data Preparation
The data is separated into two subsets for analysis: legitimate transactions (`legit`) and fraudulent transactions (`fraud`). To address the imbalance, under-sampling is performed by creating a new dataset with a balanced distribution of both classes.

### Under-Sampling
- Selected a sample of legitimate transactions to match the number of fraudulent transactions (492)
- Concatenated the sampled legitimate transactions with the original fraudulent transactions to create a new balanced dataset

## Feature Engineering
The data is split into features (`X`) and the target variable (`Y`). Features include various attributes of the transactions, and the target variable represents the transaction class (0 for normal, 1 for fraudulent).

## Data Splitting
The dataset is divided into training and testing sets using the `train_test_split` function from `sklearn`. The split is stratified to maintain the balance of classes in both sets.

## Model Training
A logistic regression model is chosen for its simplicity and effectiveness in binary classification tasks. The model is trained using the training data.

## Model Evaluation
The performance of the trained model is evaluated using accuracy scores on both the training and testing datasets.

### Logistic Regression Model
- Trained using logistic regression
- Evaluated using accuracy scores on training and testing data

## Results
- Training Data Accuracy: {training_data_accuracy}
- Test Data Accuracy: {test_data_accuracy}

## Conclusion
The logistic regression model demonstrates a promising accuracy in detecting fraudulent transactions. Further optimization and exploration of other advanced models can be considered to enhance the model's performance. Additionally, ongoing monitoring and updating of the model are crucial to adapt to evolving patterns of fraudulent activities.
