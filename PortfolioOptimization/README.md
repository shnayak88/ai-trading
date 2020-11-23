# Multi-factor Model
Build a statistical risk model using PCA. Use this model to build a portfolio along with 5 alpha factors. Create these factors, then evaluate them using factor-weighted returns, quantile analysis, sharpe ratio, and turnover analysis. At the end of the project, optimize the portfolio using the risk model and factors using multiple optimization formulations. For the dataset, we'll be using the end of day from Quotemedia and sector data from Sharadar.

Instructions 
1) Build a pipeline engine using Ziplines' pipeline. Pipeline is used to get returns data  
2) Fit a PCA model to the returns data 
3) Get factor betas, factor returns and covariance data from the PCA model
4) Use this to build the risk model -  $ \sqrt{X^{T}(BFB^{T} + S)X} $ where:
  X is the portfolio weights
  B is the factor betas
  F is the factor covariance matrix
  S is the idiosyncratic variance matrix
