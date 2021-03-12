# BankChurners

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tianqi72/BankChurners/blob/main/Classification.ipynb)

The goal of this project is to classify churning customers using supervised machine learning algorithms. I did some data preprocessing including encoding, standardization, imputation and resampling. Then I trained multiple classifiers and tune their hyperparameters through random search. After getting the best parameters, I evaluate each model using cross validation. Based on the f1 score, XGBoost has the best performance among the models. Thus, I chose it as final model and tested it on the test data. The precision, recall and f1 score are all around 0.9, which I think is a good performance.

Algorithms used:
- KNN
- SVC
- Random Forest
- XGBoost
