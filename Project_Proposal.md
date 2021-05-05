# Stock Price Prediction


### Question/Need ###
---
In this project I will be trying to predict the trend of stock price whether the price goes up or down after the period x.


### Data Description ###
---
Intraday stock data will be gathered through the IEX cloud, using their api.  
Each datapoint will contain the following features: data, minute, label, high, low, open, close, average, volumn, notional, numberoftrades.  
Provided with the features the model will predict if the price is going to increase or decrease.

### Tools ###
---
IEX api will be used for data acquisition.
Postgresql will be used for data storage.
Pandas and Numpy will be used for data manipulation.
Matplotlib and Seaborn will be used for data visualization.  
Sklearn will be used for data modeling.

### MVP Goal ###
---
All data will be cleaned with Pandas and the data will be used to model a logistic regression through sklearn.