## Apr 9	2019 CSCI 4930/5930 Machine Learning 
# Programming Assignment 3: e-commerce fraud detection

Goal: You are hired as a data scientist at a bank, say CoinBank. Let’s first imagine that. How cool would that
be! Interestingly, on your very first day at CoinBank, your are assigned a gruesome task to detect fraudulent ecommerce
transactions happening at the bank by analyzing the transaction log files.

## Dataset
Set-A.X.csv : contains information regarding the 94682 transactions.
Set-A.y.csv : target labels for each of the transaction found in the corresponding Set-A.X.csv dataset, 0 for
legitimate and 1 for fraudulent.
### Some note on the datasets
Please treat fraudulent transaction as “positive” and legitimate as “negative” sample.
Due to privacy reasons, the provider of the dataset renamed the data fields to some abstract names.
Therefore, you may treat each field equally without giving any preference to any field in the dataset.
An exploratory data analysis can be found in the provided Fraud-Detection-EDA.ipynb (jupyter notebook)
If needed, take fractions of the dataset to ac commodate into the memory capacity of your workstation.
Randomly split the SET-A dataset into 80% training and 20% test (holdout set).

## Task 1 : Logistic Regression based Classifier (LR)
#### 1. Logistic Regression based classifier construction. (Mini-batch gradient descent). Once again, do not call
library function for logistic regression fit method.
#### 1.1 Use a 10-fold cross validation strategy to obtain the best set of hyper-parameter values of the logistic
regression. Please report a discussion why you would choose the values. (On the training set)
1.2 Train the classifier on the training set, and report the training confusion matrix, accuracy, precision, recall,
F1-score, the ROC curve and the corresponding AUC score.
1.3 Using the model, test the test set, and report the testing confusion matrix, accuracy, precision, recall, F1-
score, the ROC curve and the corresponding AUC score.

## Task 2 : Naive Bayes Classifier (NB)
2. Naive Bayes Classifier construction considering the log likelihood strategy with Laplace based smoothing
for discrete variables, and Gaussian smoothing for the continuous variables to estimate the corresponding
conditional probabilities. Once again, do not call library function for Naive Bayes classification’s fit method.
2.1 We do not have any hyper-parameters to train here. Then, simply report the 5-fold cross validation
performance in terms of accuracy, precision, recall, F1-score. (On the training set)
2.2 Train the classifier on the training set, and report the training confusion matrix, accuracy, precision, recall,
F1-score, the ROC curve and the corresponding AUC score.
2.3 Using the model, test the test set, and report the testing confusion matrix, accuracy, precision, recall, F1-
score, the ROC curve and the corresponding AUC score.

## Task 3 : kNN Classifier (kNN)
3. k-NN Classifier construction (considering the normalize to unit vector strategy and Euclidean distance
measure as discussed in class). Once again, do not call library function for kNN fit method.
3.1 Use a 10-fold cross validation strategy to obtain the best hyper-parameter value of the k-NN classifier (i.e.,
the value of k). Please report a discussion why you would choose the value. (On the training set)
3.2 Train the classifier on the training set, and report the training confusion matrix, accuracy, precision, recall,
F1-score, the ROC point on the ROC space.
3.3 Using the model, test the test set, and report the testing confusion matrix, accuracy, precision, recall, F1-
score, the ROC point on the ROC space.
