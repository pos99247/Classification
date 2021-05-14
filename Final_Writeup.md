# Predicting Stock Price Trends

---

Brian Nam

## Abstract

---

The goal of this project is to use a classification model to predict stock trends for stocks in S&P 500. Stock price predictions are usually done under the following two ways:Fundamental analysis or Technical analysis. In this project we are approaching the problem with the techinical analysis. We will use historical data of stocks such as open, high, low, close, and volume. With the historical data, we will attempt to predict the price trend of stocks.

## Design

---

For each data point which is a day, we have given it a target column. The target  variable is the mean of the percentage change in the closing price for 5 subsequent days. Then the depending on whether the target column is a positive or a negative, it is labeled as 1 or 0 respectively. 

## Data

---

The dataset contains 349,948 data points of historical stock data from 2018-07-13 through 2021-04-26 with 6 features. The features are open, high, low, close, adjusted close, and volume. By implimenting the technical analysis library, we were able to add 85 additional features. Target variable is a binary variable of 1 or 0, which means a upward trend or downward trend respectively.


## Algorithms

---
**Feature Engineering**
By aggregating past historical data, we were able to create important features such as volatility, trend mass index, and price rate of change indicator.

**Models**
Logistic regression was used for initial modeling. To increase model accuracy, grid search was used to increase accuracy. Xgboost and random forest was also used to model.

**Evaluation Metric**
Accuracy was chosen as the main metric. Confusion metric was chosen to support the accuracy metric in order to prove the model is not selecting only one class. 

**Model Evaluation**
The entire data set was split into 6:2:2 = Train:Valid:Test. Then the xgboost model was refitted with the entire set then was used to predict the test set.  
Xgboost : Test set Accuracy : 0.5530, Train set Accuracy : 0.5525.

## Tools

---

* Yahoo Finance api for webscraping
* Sqlite for data storage
* Pandas and numpy for data manipulation
* Seaborn and matplotlib for data visualization

## Communication

---

Slides were made for the presentation to give a better understanding of the model.