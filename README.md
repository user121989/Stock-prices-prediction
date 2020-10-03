# Stock-prices-prediction

## Project tasks:
1) Create an investment portfolio with a high level of returns and relatively low volatility. To solve this task we will use the next strategy:
compute daily returns for every financial tool;
* calculate the mean and variance of the daily returns for every financial tool;
* generate 10 000 random sets of weights. Thus we will have 10 000 variants of portfolio structure with different shares of financial tools;
* among all 10 000 portfolios, we will choose one with the highest level of profit and relatively small volitation.
2) Predict stock prices for the next 5 days with the Monte Carlo method and with ML algorithm.
__Monte Carlo Method__ - this algorithm includes a simulation of 1000 random returns for each of the 5 required days. Based on this method we can plot the probability density function and cumulative distribution function, which will show us the probability of the specific level of profit (for example probability to earn more than 5 percent per day). Moreover based on generated by this method data we can compute the expectation of stock price for every day.n\
__Machine Learning algorithm__. We will take the simplest one – Linear Regression. For this algorithm, we need to have independent variables and dependent feature. To create a dependent feature we will copy downloaded stock data but shift it for the 5 days forward. Thus we will try to predict based on the stock price in one day what would like it be five days later.

## Data desription
For this project stock market data from yahoo was used. In particular prices of FAANG (Facebook, Apple, Amazon, Netflix, Google) shares were taken into account, moreover, gold and oil quotations were added to the project as an alternative way of investment. The analyzing period starts from 01.01.2014 and ends on 31.08.2020. This period can be characterized as unstable thus it's more interesting how ML algorithm and Monte Carlo method will handle the task.
