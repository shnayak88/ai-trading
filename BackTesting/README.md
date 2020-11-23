# Backtesting Alpha Factors using Barra Data 

The backtester will perform portfolio optimization that includes transaction costs, and  implement it with computational efficiency 
in mind, to allow for a reasonably fast backtest. It will also use performance attribution to identify the major drivers of 
the portfolio's profit-and-loss (PnL). 

Instructions 
1) Use Barra dataset to load factors to predict risk 
2) Use OLS to estimate factor returns given returns and factor exposures
3) We will choose 4 alpha factors - Reversal, Earnings Yield, Value and Sentiment 
4) Build Universe Filters: Companies that have a market capitalization of at least 1 billion dollars OR that are in the previous day's holdings, even if on the current day, the company no longer meets the 1 billion dollar criteria
5) Perform the optimization (scipy optimization library), objective function: 
Minimize factor risk + idiosyncratic risk - expected portfolio return + transaction costs
6) Run the backtest - Walk through each day, calculating the optimal portfolio holdings and trade list
7) Profit and Loss is the aggregate realized daily returns of the assets, weighted by the optimal portfolio holdings chosen, and summed up to get the portfolio's profit and loss.
  a) The PnL attributed to the alpha factors equals the factor returns times factor exposures for the alpha factors.
  b) Similarly, the PnL attributed to the risk factors equals the factor returns times factor exposures of the risk factors.





