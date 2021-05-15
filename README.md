# DLfinalproject
Algorithm comparison in stock price prediction

The code used for the experiment is in the AlgoComparisonNotebook.ipynb

It is seperated into following parts:
- data preprocessing using web scraping and visulization on the data internal correlation
- Regressor model run for the cross-company prediction (with prediction graph and RMSE)
- Auto Arima run for Lululemon's part performance (with prediction graph and RMSE)
- Prophet run for Lululemon's part performance (with prediction graph and RMSE)
- LSTM run for Lululemon's part performance (with prediction graph and RMSE)
- ANN model combine the results from LSTM and Regressor to do predition on High and Low

##Except the preprocessing, each step generates the RMSE and graphs for performance evaluation


This repo contains the following files/folder:
- stock_details: web scraping results of the ten companies
- tickers.pickle: storing companies' names for web scraping
- RNN_results.csv: prediction result of RNN (LSTM)
- RNN_model.h5: saved RNN model
- Regressor_results.csv: prediction results for Regressor
- Regressor_results_mod.csv: trancated result for combined model
- Regressor_model.h5: saved Regressor model
- features.csv: for the purpose of histogram of regression
- Dataset_temp.csv: saving web-scraped data
- Dataset_target.csv/Dataset_target_2.csv: Lululemon's data (our target company)
- Dataset_main.csv: all stock data
- AUTOARIMA_result.csv: prediction result of auto arima
- ANN_model.h5: saved ANN model