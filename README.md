# Stock-Prices
Two Datasets were used:
* historical_stock_prices
* historical_stocks

source [Stock-Prices](https://www.kaggle.com/ehallmar/daily-historical-stock-prices-1970-2018?fbclid=IwAR0mkRuSU1u5GSJDSBPmKbAsJa1gnfJ7GSjYOxuSrqwMwFfNa0UgUzKfhUk)

## Objetivos
This study intends to make a forecast prediction of the adjusted closed price of several companies. 
First of all, we intend to analyze the dataset, evaluate the sectors of the predominant companies on the market as other factors as volume stocks, open prices.. all features that can be possible correlated with what we want to predict.
In adition, if necessary we intend to enrich the dataset with all the information we can find that will help us to improve stock forecasting for certain companies.


Subsequently, use several traditional machine learning models to predict these adjusted closed prices such as linear models, decision trees, SVM...
Secondly, use Deep Learning algorithms, namely RNN and LSTM/GRU to compare results with the first approach.

Finally, tune our models and draw relevant conclusions.

## historical_stocks


| 					  |  ticker  			|	exchange	|	name									|	sector	 		 |	industry				  |
| ------------------- | ------------------- | ------------- | ----------------------------------------- | -------------------| -------------------------- | 
|  0				  |  PIH				|	NASDAQ		|	1347 PROPERTY INSURANCE HOLDINGS, INC.	| FINANCE	 		 | PROPERTY-CASUALTY INSURERS |
|  1				  |  PIHPP				|	NASDAQ		|	1347 PROPERTY INSURANCE HOLDINGS, INC.	| FINANCE	 		 | PROPERTY-CASUALTY INSURERS |
|  2				  |  TURN				|	NASDAQ		|	180  DEGREE CAPITAL CORP.				| FINANCE	 		 | FINANCE/INVESTORS SERVICES |
|  3				  |  FLWS				|	NASDAQ		|	1-800 FLOWERS.COM, INC.		 			| CONSUMER SERVICES	 | OTHER SPECIALTY STORES 	  |
|  4				  |  FCCY				|	NASDAQ		|	1ST CONSTITUTION BANCORP (NJ)			| FINANCE	 		 | SAVINGS INSTITUTIONS 	  |

We realize there are 5 columns and this dataset:
* **ticker** corresponds to the name of the share
* **exchange** corresponds to the type of exchange made
* **name** refers the company's name
* **sector** refers to the actual sector where the given company operates
* **industry** specifies the type of services that can be provided

## historical_stock_prices

| 					  |  ticker  			|	open	|	close	|	adj_close  |	low	 |  high  |  volume |    date      |
| ------------------- | ------------------- | --------- | --------- | ------------ | ------  | ------ | ------- | ------------ |
|  0				  |  AHH				|	11.50	|	11.58	| 	8.493155   |  11.25  | 11.68  |  4633900|  2013-05-08  |
|  1				  |  AHH				|	11.50	|	11.55	| 	8.471151   |  11.50  | 11.66  |  275800 |  2013-05-09  |
|  2				  |  AHH				|	11.50	|	11.60	| 	8.507822   |  11.50  | 11.65  |  277100 |  2013-05-10  |
|  3				  |  AHH				|	11.50	|	11.65	| 	8.544494   |  11.55  | 11.60  |  147400 |  2013-05-13  |
|  4				  |  AHH				|	11.50	|	11.53	|   8.456484   |  11.50  | 11.60  |  184100 |  2013-05-14  |
|  ...				  |  ...				|	...		|	...		| 	...		   |  ...    | ...	  |  ...	|   ...		   |
|  20973884			  |  NZF				|	14.60	|	14.59	| 	14.590000  |  14.58  | 14.62  |  137500 |  2018-08-20  |
|  20973885			  |  NZF				|	14.60	|	14.58	| 	14.580000  |  14.57  | 14.61  |  151200 |  2018-08-21  |
|  20973886			  |  NZF				|	14.58	|	14.59	| 	14.590000  |  14.57  | 14.63  |  185400 |  2018-08-22  |
|  20973887			  |  NZF				|	14.60	|	14.57	| 	14.570000  |  14.57  | 14.64  |  135600 |  2018-08-23  |
|  20973888			  |  NZF				|	14.60	|	14.69	| 	14.690000  |  14.59  | 14.69  |  180900 |  2018-08-24  |


This dataset contains 8 columns:
* **ticker** corresponds to the name of the share
* **open** describe the open price of that share in a specific day
* **close** describe the final share price in the end of a day
* **adj-close**  it´s a tricky column, describes the ajudsted price of a share, thats normally different from the close price
	- An example of this, is when a stock splits occur. A stock split it's a current way used for compannies to sell more stocks, by diving the price in (x), lets say x = 2, then if one share = 10€, then, when stock split occurs, let say with a split=2, the share is equal to 5€, but in the end this 2 shares represent the same as 1 share, e.g, imagine that the companny have 10 shares, if you buy 1 share you have 1% of the company, in a stock split(split=2), if you buy 2 shares you only have 1% of the comapnny two.
	- A stock's price is typically affected by supply and demand of market participants. However, some corporate actions, such as stock splits, dividends / distributions and rights offerings can affect a stock's price and adjustments are needed to arrive at a technically accurate reflection of the true value of that stock.
* **low** is the lowest value paid for that share
* **high** is the highest value paid for that share
* **volume** represents the shares purchased in that day
* **date** represents the date (year-month-day)



# Machine Learning Algorithms

1. Linear Regression
2. Support Vectors Classifers for Regression SVR
3. Decisions Tree / Random Forest
4. Recurrent Neural Networks (RNN) / LSTM

# Group

* André Guilherme Nunes Viveiros - a81736
* Guilherme Marques Andrade – a80426
* Rodrigo Teixeira Pereira – pg38424


