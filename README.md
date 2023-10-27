# Taxi Orders Next Hour Forecasting

## Project Description
A machine learning model is needed for a taxi application to predict the number of taxi orders for the next hour. The goal is to attract more drivers during peak demand periods. Historical data on taxi orders is available.  

## Key Findings
Data preprocessing was carried out, including resampling and decomposition into trend, seasonality, and residuals.  
A pattern of daily and weekly cyclicality in taxi orders was identified.  
Additional features were created, including:  
- Calendar features (month, day, day of the week, hour).
- Lag features (time-shifted by various hours).
- Moving average.
  
The best value of the target RMSE metric was achieved using an LGBM model with the following hyperparameters:
- Learning_rate': 0.05  
- N_estimators': 100  
  
On the test dataset, an RMSE value of 41.90 was achieved, which is better than the target value of <= 48.  

## Additional Information
Toolkit: Pandas, Python, LightGBM, Scikit-learn, statsmodels
