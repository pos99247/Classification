# Stock Price Prediction


### Question/Need ###
---
In this project I will be trying to predict the trend of stock prices for stocks in S&P 500. 


### Data Description ###
---
Daily trading data of 505 stocks in S&P 500 will be collected.
Daily stock data will be gathered through the IEX cloud, using their api.  
Each datapoint will contain the following features: data, minute, label, high, low, open, close, average, volumn, notional, numberoftrades, peak in 1 year, lowest in 1 year, moving average, adjusted closing price, previous closing price, and company fundamental data. 
The fundamental data will include things such as divideneds, price to earning ratio, and other miscellaneous data of the company. 
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
Extensive feature engineering will be done. Examples will be various closing price depending on time and different moving averages.
Then the data set will be fitted into a logistic regression as the base model.