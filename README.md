# Model: LSTM
Long Short-Term Memory (LSTM) was designed to address the vanishing gradient issue faced by traditional RNNs when learning long-term dependencies in sequential data. LSTMs are capable of maintaining information over extended periods because of memory cells and gating mechanisms.
# Dataset: This hourly data set contains the PM2.5 data of the US Embassy in Beijing. Meanwhile, meteorological data from Beijing Capital International Airport are also included.

Dataset Characteristics: Multivariate, Time-Series

Subject Area: Climate and Environment

Associated Tasks: Regression

Feature Type: Integer, Real

Instances: 43824

Features: 11

There are 2067 missing values in the column pm 2.5. (PM stands for particulate matter, a mixture of solid particles and liquid droplets found in the air. PM2.5 are fine particles that pose the greatest risk to health and visibility. )
* No: row number
* year: year of data in this row
* month: month of data in this row
* day: day of data in this row
* hour: hour of data in this row
* pm2.5: PM2.5 concentration (ug/m^3)
* DEWP: Dew Point (â„ƒ)
* TEMP: Temperature (â„ƒ)
* PRES: Pressure (hPa)
* cbwd: Combined wind direction
* Iws: Cumulated wind speed (m/s)
* Is: Cumulated hours of snow
* Ir: Cumulated hours of rain

# Outliers: 
In time-series data like the Beijing PM2.5 dataset, backward fill (bfill) and forward fill (ffill) are simple but effective strategies to handle missing values.

# Regression model evaluation metrics

The MSE, RMSE, and R-squared metrics are mainly used to evaluate the prediction error rates and model performance in regression analysis.

* MSE (Mean Squared Error) represents the difference between the original and predicted values extracted by squaring the average difference over the data set.
* RMSE (Root Mean Squared Error) is the error rate by the square root of MSE.
* R-squared (Coefficient of determination) represents the coefficient of how well the values fit compared to the original values. The value from 0 to 1 is interpreted as percentages. The higher the value is, the better the model is.

# Result:
* Final model Validation loss: 0.0005462467088364065
* Final Model RMSE: 0.0247
* Final Model R-squared: 0.9308
* The overall performance of the model improves after the learning rate scheduler.
      
In the loss curve,
* Validation Loss is consistently low and flat after a few epochs.


  
