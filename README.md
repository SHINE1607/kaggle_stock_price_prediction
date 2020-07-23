# kaggle_stock_price_prediction

## Problem Statetment

To develop a machine learning model pedict future stock price  using historical data

## Data Matrix

The data matrix is of the shape (851264, 7), called prices.csv 
prices.csv has features:
* date: The date feature
* symbol : symbol of the firm in the NYSE list
* close: the closin value for the day
* open: the openeing value for the day 
* low: the lowest value of stock for the day
* high: the highest value of stock for the day
* volume: total volume od stockes traded for the day

The stock prices listed are in th range ('2010-01-04', '2016-12-30') for a period of six years
###  There are total of 501 companies in the dataset and we are training a model for the oracle closing stock prices using LSTM Deep learning model

## Plot of the closing stock price for oracle from 2010 to 2016

![alt text](https://github.com/SHINE1607/kaggle_stock_price_prediction/blob/master/images/actual_plot.PNG)

## Data Preprocessing
Not much of data preporcessing needed, just we are scaling down the stock price to decrease the variance in the data using minmaxscalar

## Model used and Model  architecture

The model used to train the data is LSTM that takes timesteps of 100 to predit the succeeding value
In simple terms, preceding 100 days closing values will be the features for the next day
### model architecture is hsown below
![alt text](https://github.com/SHINE1607/kaggle_stock_price_prediction/blob/master/images/model_archituecture.PNG)
 
## validation data prediction and plotting the predicted data
### Plot of comparison of predcited data and actual data vs timeframe
![alt text](https://github.com/SHINE1607/kaggle_stock_price_prediction/blob/master/images/final_plot.PNG)
###  performance and model evaluation
estmiated mse value for test data : 31.935114583766264




