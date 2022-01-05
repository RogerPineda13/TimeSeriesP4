# TimeSeriesP4
This repo is to show our inner working with Time Series Modeling


# Overview
This project uses Time Series Analysis and Time Series Modeling to accurately predict the current/future stock price of pre-selected companies. The purpose for this time series model is so that we can advise our investors when to put their money into the market.

We will be focusing on data collected from January 2006 until January 2018. This dataset is consistent of entries when the stock market is open


# Business Understanding & Key Questions
The ever wanting answer to everyone who wants to turn their money into more money is when is the right time to invest my money into the stock market. Timing is crucial when it comes to stocks and investing. Putting in your money when the market is reaching a peak and will only go down could cost you your life savings. Taking your money out too early could make you miss out on capital gains that could finance the start of a new journey. You as a future investor could possibly use our model to find out the future price of a stock.  


* Is it possible to predict future stock prices by just looking at the past?
* How significant is looking at the closing price for a stock for the day play into the future price?
* Is it the right time to invest?
# Behind Our Data Decisions
The following dataset was grabbed from kaggle and was used to build our model.
* DJIA_equities/CSCO_2006-01-01_to_2018-01-01.csv


When thinking about time series, the first objective of the modeling process is to have a data set that is fully cleaned meaning there aren’t any null/NaN values and that the features that are left in our data frame are only values we plan on fully utilizing for processing. With our dataset, we were fortunately given the following: 
* opening 
* closing 
* low 
* high 
* ticker 
* volume 

For each of the 30 constituents that make up the Dow Jones Index. For the sake of our predictions, we wanted to use the closing price which is a strong indicator for the following days as it is reflective of all news what occurred that day, and can also be indicative of the opening price the following day given market conditions. If the close is higher than the prior open or prior day close, it generally will mean a strong market indicator that the price will continue to run given some string of good news around the equity. An example of this would be a company reporting strong earnings as of a prior quarter or announcing a new product such as a new range of iPhone for Apple. 

To drill down the data a bit further, we decided to focus specifically on one equity, CSCO or formally known as Cisco Systems, Inc. Cisco is a multinational company conglomerate that develops and sells software, hardware and other high end technology systems. CSCO historically has fluctuated around 20-30 dollars in the mid 200s and early 2010s however they’ve seen a steady increase in the last 5 years 2016-2022 to a price around 60 dollars now. We decided this would be a good data set to use as it was somewhat stationary already however it would test our time series prowess to see if we could predict data we split from around 2016-2018.

# Modeling

# Recommendations & Conclusions
