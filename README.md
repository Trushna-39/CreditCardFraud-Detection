# Credit Card Fraud Detection

## Project Overview
This project aims to detect fraudulent credit card transactions using a highly imbalanced dataset. The dataset consists of transactions made by European cardholders in September 2013. Out of 284,807 transactions, 492 are fraudulent, which constitutes approximately 0.172% of the data.

## Dataset Description
The dataset for this project is taken from Kaggle: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud. <br/>
The dataset includes transactions from a two-day period. Due to confidentiality reasons, the original features of the transactions cannot be provided. Instead, the data consists of numerical input variables resulting from a PCA (Principal Component Analysis) transformation.

## Features
1. V1, V2, ..., V28: Principal components obtained through PCA.
2. Time: The seconds elapsed between each transaction and the first transaction in the dataset.
3. Amount: The transaction amount, useful for example-dependent cost-sensitive learning.
4. Class: The response variable indicating whether a transaction is fraudulent (1) or not (0).

## Key Points
The dataset is highly unbalanced, with fraudulent transactions making up only 0.172% of all transactions.
The features Time and Amount are not transformed by PCA.
Due to the imbalance, standard accuracy metrics are not suitable for this problem.

## Model Selection and Training
Since the classes are either Normal Transactions - labeled as 0, or Fraud Transactions - labeled as 1 in the dataset, Logistic Regression model was the suitable choice for binary classification.

## Evaluation Metrics
The Logistic Regression Model is evaluated using the accuracy as a metirc that matches the actual targets and predicted targets.
