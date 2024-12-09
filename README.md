# Stock Price Sentiment Analysis

## Overview
This project forecasts the directional movement of the Dow Jones Industrial Average (DJIA) by integrating sentiment analysis with historical stock market data. Sentiment scores, derived from the top 25 daily Reddit headlines using VADER (Valence Aware Dictionary and Sentiment Reasoner), are combined with stock price indicators to enrich predictive features. Machine learning models, including Support Vector Machines (SVM), Logistic Regression, Naive Bayes, Linear Discriminant Analysis (LDA), and Random Forest, are trained on data from 2008–2015 and evaluated on 2016 data.

## Components
### Data
- Source: https://www.kaggle.com/datasets/aaron7sun/stocknews/code
- Contents:
  - Historical stock prices.
  - Daily top Reddit financial news headlines ranked by user votes.

### Features
- Stock Market Features: Opening Price, High, Low, Closing Price, Adjusted Close Price, Volume.
- Sentiment Score: Extracted using the VADER sentiment analysis tool.

### Preprocessing
Text headlines were cleaned by removing special characters, URLs, and unnecessary symbols. Lagged features were created to ensure predictions rely only on past data.

### Models
The following machine learning models were implemented and evaluated:
- Logistic Regression.
- Linear Discriminant Analysis (LDA).
- Random Forest.
- Naive Bayes.
- Support Vector Machines (SVM).

### Evaluation Metrics
- Precision-Recall Curve (PRC): Evaluates precision and recall balance for imbalanced datasets.
- ROC Curve: Measures True Positive Rate (TPR) vs. False Positive Rate (FPR).
- Accuracy, Precision, Recall, and Area Under Curve (AUC).
