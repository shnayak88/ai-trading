# Combine Signals for Enhanced Alpha
In this project, we combine signals on a random forest for enhanced alpha. While implementing this, we'll have to solve the problem of overlapping samples. For the dataset, we'll be using the end of day from Quotemedia and sector data from Sharadar.

Instructions:
1) Going to use the quantopian pipeline to load the data. We are going to use the following features <br/> 
  a) "Universal" Quant Features. To capture the universe, we'll use the following as features:<br/>
  Stock Volatility 20d, 120d <br>
  Stock Dollar Volume 20d, 120d <br/>
  Sector <br/>
  b) Regime Features <br/>
  High and low volatility 20d, 120d <br/>
  High and low dispersion 20d, 120d <br/>

2) One Hot Encode Factors: For the model to better understand the sector data, we'll one hot encode this data.
3) Build a Random Forest Classifier, classifying the stocks based on the above factors
4) Handle the overlapping samples problem. <br/>
    a) Don't use overlapping samples <br/>
    b) Use BaggingClassifier's max_samples <br/>
    c) Build an ensemble of non-overlapping tree <br/>
5) Run the model on training, validation and test
6) You will see that the combined signal alpha performs better than other factors based on sharpe ratio 



 

