# GARCHTImplementation
GARCH


# StockPricePredictionUsingLSTM
LSTM Price Movement Predictions For Trading Algorithms
 This Code focuses on collecting dataset and train LSTM RNN Model to predict.
 Currently it has following technical indicators:
      - RSI
      - EMAF
      - EMAM
      - EMAS
      

Low TODOs:
   - Implement Various GARCH Models such as:
     -   Univariate GARCH ,
     -   Multivariate GARCH
   - Implement SHAP framework fromm the following example:
     - https://www.geeksforgeeks.org/shap-a-comprehensive-guide-to-shapley-additive-explanations/  

 Complex TODOs:
   - Apply the following performance metrics, including: 
       - MAE : Mean Absolute Error
       - RMSE: Root Mean Square Error
       - MAPE: Mean Absolute Percentage Error
       - and R-squared.
   - This is a comment from one of the advance youtube videos:
   -  "ive got a 6 gb csv file with the last 5000 days of price info for around 4800 companies merged with quarterly financial data like assets revenue etc merged with macro indicators like interest rates and all of that interpolated and cleaned up before passing to an lstm with many many layers with tuned hyper params. instead of using a standard loss value you should use mean absolute percentage error because if a stock is trading at 1$ and you have a loss of 1$ you would be off by 100% but if its trading at 1000$ and yoru loss is 10 then you would be off by 1%.

also try to use time distributed lstm layers at the input and to use leaky relu not just relu so that parts of the model that arnt use often dont just become dead weight . Also use a deeper model to capture the complex relationship between the columns in the training data and MOST IMPORTANTLY..... Kill any over fitting with lots of dropout layers and batch norm"
