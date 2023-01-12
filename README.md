# Algo-Trading-Homework
The main task in this challenge is to use machine learning to enhanced existing trading signals in an automated trading algorithm.

### Organization
The relavent python notebooks is titled `machine_learning_trading_bot.ipynb`

### Code and Dependencies
This code is to be run on `Python 3.7.13`

The following Python Libraries were also imported and used:

`import pandas as pd`
`from path import Path`
`import numpy as np`
`import hvplot.pandas`
`import matplotlib.pyplot as plt`
`from sklearn import svm`
`from sklearn.preprocessing import StandardScaler`
`from pandas.tseries.offsets import DateOffset`
`from sklearn.metrics import classification_report`

## Objectives
- Establish a Baseline Performance of the algorithm
- Tune the Baseline Trading Algorithm
- Evaluate a New Machine Learning Classifier

## Model Evaluation
The initial classifier model used was SVC from sklearn, which is a type of support vector machine learning method, which calculates the best hyperplane to seperate data into different classes. By evaluating this model's precsion and recall, we found that is performed worse at predicting whent to short that it did at predicting when to buy (whihc itself was only slightly above 50%). The recall was also only 4% for shorting. 

The second model we created was created using Bayesian Ridge Regression. One of the main advantage of Bayesian Ridge Regression is applying the model in cases where you want to quantify the uncertainty in your predictions. Since there is significant uncertainty in stock price movement, this was selected for testing.

## Conclusion
