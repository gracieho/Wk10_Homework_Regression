# Week 10 Homework Assignment - A Yen for the Future

### Time Series Analysis
We reviewed the long term trend of the Yen saw that it had a upward trend and was non-stationary (as demonstrated by the Augmented Dickey-Fuller test.

The historical Yen data was then decomposed using the Hodrick-Prescott Filter into the trend and the non-trend (or noise) components.

We then looked to forecast the Yen for the next 5 days using an ARMA model, an ARIMA model and a GARCH model.  The ARMA and ARIMA model's P values were all significantly higher than 0.05, indicating those models were not useful in predicting the Yen's future values.  While the GARCH model's P values were smaller than 0.05, I would not use these models to determine Yen trading strategies, as past prices are  not necessarily a good predictor of future Yen prices, as there are more than simple historical price trends which impact Yen values. 

### Regression Analysis
We then applied a Linear Regression on the Yen data and it's returns, separating the dataset into a training set and a testing set (based on years).

We calculated the Root Mean Squared Error (RMSE) of the In sample vs Out of sample data.  While normally one would expect the in sample data to have a lower RMSE than the Out of sample data, this was not the case with our model. 

We performed one additional test - which was to obtain the RMSE of a simple mean of the data as a comparison point.  The RMSE of the mean of the data was marginally better than the out of sample RMSE, indicating that the model's ability to predict values was no better than using a mean of the data.  That is, the model is not very useful.