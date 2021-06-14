# Predicting Churning Customers

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tianqi72/BankChurners/blob/main/Classification.ipynb)

## Introduction
Banks often face customer churn, which means loss of customers. Attracting new customers costs more than retaining existing customers, so it is helpful for managers to predict who will leave the services and thus take proactive actions to persuade customers to stay. The goal of this project is to predict whether credit card customers will get churned using supervised machine learning algorithms. 

### Dataset
- Source: Kaggle (https://www.kaggle.com/sakshigoyal7/credit-card-customers)
- Shape: 10127 rows, 20 columns
- Target: Existing Customer(84%)/Attrited Customer(16%)
- Features:
  - Age
  - Dependent
  - Education Level
  - Income
  - Credit limit
  - Month on book
  - etc.

### Methods Used
* Machine Learning (Binary Classification)
  - KNN
  - SVC
  - Random Forest
  - XGBoost
* Data Visualization
* Resampling
* Hyperparameter Tuning

### Technologies
* Python
  - Pandas
  - Numpy
  - Matplotlib
  - Sklearn
    - Pipeline
    - StandardScaler
    - OneHotEncoder
    - LabelEncoder
    - SimpleImputer
    - cross_val_score
    - RandomizedSearchCV
  - Imblearn
    - SMOTE

## Project Description
In this project, I did some data preprocessing including encoding, standardization, imputation, all of which are done within sklearn pipeline. As the dataset is imbalanced, I used resampling method SMOTE. Then I trained multiple machine learning classifiers and tuned their hyperparameters through random search. After getting the best parameters, I evaluated each model using cross validation. Based on the f1 score, XGBoost has the best performance among the models. Thus, I chose it as final model and tested it on the test data. The precision, recall and f1 score are all around 0.9, which is a good performance.
