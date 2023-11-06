# Investment_Trading_Capstone_Project

## Motivation for the project:
I always was interested if it is possible to predict stock prices. I was curious if python and machine learning techniques can support me in this query and make the predictions better. That I what I would like to study in my project.


## Project Overview:
In my capstone project I am exploring the movements of stock prices and applying some machine learning technics, trying to predict the movements of stock prices.

Data I use is from yahoo finance. As input I take daily trading data: opening price (Open), highest price the stock traded at (High), how many stocks were traded (Volume) and closing price adjusted for stock splits and dividends (Adjusted Close).

First I am looking at the development of adj close stock prices by means of comparing a visualising different trading parameters: Daily returns, Cumulative returnes, Rolling statistics of mean, standard deviation and Bollinger Bands, as well as MACD and RSI. These parameters show, how risky (or volatile) are the stock prices, how profitable they are and what investing logic could be used. Several of these techniques indeed have some power to predict stock prices movements.

After looking at the trading parameters, I am going forward in my analysis of stock prices movements by means of machine learning models. First I am using Classifiers to predict if Adjusted Close price is going up or down the next day for single stock. After that I am using Regressor models trying to predict the value change. As features I am using the trading parameters I explored in the previous part and lag values of the previous days. I am comparing different features, looking which set of them and for which period have the highest predictive power. I am also checking the models I would suggest to use for predictions for robustness, by testing them ob different stocks and for different time periods.


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
1 Capstone Project Stock Forecasting jupyter file of the project with all visualisations, explanaitions and details
2 Capstone data.csv sample dataset with stock prices data and calculated parameters


## Summary of the results of the analysis:
In my research I tried to forecast stock prices. For that I used different Machine Learning models. Classification models seem to deliver very resilts with high predictive power of up to 80% on if a stock price is going to grow or fall the next days. Model that delivered the best results was Random Forest Classifier after tuning of its parameters (number of trees, minimum number of features to consider when looking for the best split and required to split an internal node, maximum depth of the tree and if or nor using Bootstraping. I got really great results using trading parameters (MACD and Signal, Rolling mean and standard deviation, RSI and Williams %R), that already according to their visualisation looked promising to predict price movements. Tuned model worked great for different time periods and for different stocks. It turned out that longer time periods doesnt contribute to higher predicive power of the model. Also just taking laged values of returnes doest make the predictions better. It also goes hand in hand with the fact that ARIMA model didnt work for predictions as it is baced on correlation between present and laged past values of stock prices.


