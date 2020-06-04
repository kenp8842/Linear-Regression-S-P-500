# Linear Regression S & P 500: Project Overview

* Created a model (RMSE ~ 16) to estimate the closing price for the S & P 500 to show ability in linear regression
* Used existing data that contained the open, high, low, and closing price as well as the daily volume
* Created four different features for our model involving closing price and volume information
* Used a linear regression model to predict closing prices on our test set and evaluated model performance in different ways

## Code and Reference Used

**Python Version**: 3.7                                                         
**Packages**: pandas, numpy, matplotlib, sklearn

## Resources

### Data
https://raw.githubusercontent.com/NickyThreeNames/DataquestGuidedProjects/master/Guided%20Project-%20Predicting%20the%20stock%20market/sphist.csv

### Stock Market Definitions
https://en.wikipedia.org/wiki/S%26P_500_Index                           
https://en.wikipedia.org/wiki/Volume_(finance                                             
https://www.investtech.com/main/market.php?CountryID=44&p=staticPage&fn=helpItem&tbReport=h_PVC

## Data Cleaning

The data cleaning involved getting our dates into datetime objects and reversing the index of the dataframe so we it was listed from
earliest to most recent price.

## Feature Engineering

Created the following four features for our model:                                      
* 5 day closing price average
* 30 day closing price average
* ratio of the standard deviation of the closing price for the previous week to the previous year
* ratio of the standard deviation of volume for the previous week to the previous year

## Model Building

I used a linear regression model, as it was the purpose of this exercise.

## Model Performance

The RMSE of our model on the test set was apporximately 16. I also tried to evaluate using this type of model in some form of a trading
system even though it lags behind price during well defined trends either up or down. The model does fairly well establishing turns or
trend changes in the stock market. This can be seen graphically below.

![](https://github.com/kenp8842/Linear-Regression-S-P-500/blob/master/sp_500_perform.png)
