# Investment_Trading_Capstone_Project

## Motivation for the project:
I always was interested if it is possible to predict stock prices. I was curious if python and machine learning techniques can support me in this query and make the predictions better. That I what I would like to study in my project.


## Project Overview:
In my capstone project I am exploring the movements of stock prices and applying some machine learning technics, trying to predict the movements of stock prices.

Data I use is from yahoo finance. As input I take daily trading data: opening price (Open), highest price the stock traded at (High), how many stocks were traded (Volume) and closing price adjusted for stock splits and dividends (Adjusted Close).

First, I am looking at the development of adj close stock prices by means of comparing a visualising different trading parameters:, Cumulative Stock Returnes, Rolling statistics of mean, standard deviation and Bollinger Bands, as well as MACD and RSI. These parameters show, how risky (or volatile) are the stock prices, how profitable they are and what investing logic could be used. Several of these techniques indeed have some power to predict stock prices movements.

After looking at the trading parameters, I am going forward in my analysis of stock prices movements by means of machine learning models. First, I was using Classifiers to predict if Adjusted Close price is going up or down the next day for single stock. After that, I was using Regressor models trying to predict the value change. As features I was using the trading parameters I explored in the previous part and lag values of the previous days. I am comparing different features, looking which set of them and for which period have the highest predictive power. I am also checking the models I would suggest to use for predictions for robustness, by testing them ob different stocks and for different time periods.


## Installations:
to get the stock market information you need to pip install yfinance

pip install yfinance

I did my project on thePython 3.11.4 version of Python and used the following libraries:

pandas
numpy
random
matplotlib
datetime
tqdm
sklearn
statsmodels


## Files Descriptions:

1 investment_trading_capstone_project.ipynb jupyter file of the project with all visualisations, explanaitions and details

2 Capstone data.csv sample dataset with stock prices data and calculated parameters


## Summary of the results of the analysis:
I tried to forecast stock prices. For that I used different Machine Learning models. Classification models seem to deliver very resilts with high predictive power of up to 70% on if a stock price is going to grow or fall the next days. Model that delivered the best results was Random Forest Classifier. I got really great results using trading parameters (MACD and Signal, Rolling mean and standard deviation, RSI and Williams %R), that already according to their visualisation looked promising to predict price movements. Also, just taking laged values of returnes doest make the predictions better. It also goes hand in hand with the fact that KNeighborsRegressor, Linear Regression, Ridge Regression models didnt work for predictions.

## Difficulties that I accounted during my project.

One of the difficulties I had is regarding the content. I had to do some research and found a lot of sources explaining how stock market works and how to calculate some trading parameter (including Machine Learning source for trading, suggested by Udacity, that was interesting and expanded my understanding of stock market), but I didn’t find any good source explaining which machine learning models are best to use for trading. I tried a lot of different models, but most of them gave bad accuracy results, I found a lot of tries but none of them demonstrated good performance or was explained why one works better than another. Even in books for machine learning I couldn’t find it. And the last thing that was difficult is to stop trying more and more new models using more and more datasets.

## Acknowledgments

My medium article to this project: https://medium.com/@katrina.hramovich/-d0f21a502a35.

Many thanks to Udacity for giving me an opportunity to try out real world problems and referencing the Machine Learning for Trading course https://www.udacity.com/course/machine-learning-for-trading--ud501 that gave me some insights into trading.

This project was completed as part of the Udacity Data Scientist Nanodegree program.

References:

1)Popular Classification Models for Machine Learning: https://www.analyticsvidhya.com/blog/2020/11/popular-classification-models-for-machine-learning/ 

2)Top 5 Machine Learning Practices Recommended by Experts: https://www.kdnuggets.com/2022/09/top-5-machine-learning-practices-recommended-experts.html

3)Tips and tricks to tune hyperparameters in machine learning that help improve model accuracy: https://towardsdatascience.com/hyperparameter-tuning-in-python-21a76794a1f7 



