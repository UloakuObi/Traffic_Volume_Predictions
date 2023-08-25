# Traffic-Volume-Predictions

This project focuses on analyzing the hourly traffic volume data for westbound I-94 in Minneapolis-St. Paul, MN, spanning from 2012 to 2018. This dataset contains not only traffic volume but also includes weather and holiday-related features. 

My primary objective is to identify key indicators of heavy traffic on this stretch of the I-94 Interstate highway. The aim is to uncover patterns that contribute to increased traffic congestion by investigating various factors such as weather conditions, time of day, and day of the week.

## Data Dictionary
* `holiday` Categorical US National holidays plus regional holiday, Minnesota State Fair
* `temp` Numeric Average temp in kelvin
* `rain_1h` Numeric Amount in mm of rain that occurred in the hour
* `snow_1h` Numeric Amount in mm of snow that occurred in the hour
* `clouds_all` Numeric Percentage of cloud cover
* `weather_main` Categorical Short textual description of the current weather
* `weather_description` Categorical Longer textual description of the current weather
* `date_time` DateTime Hour of the data collected in local CST time
* `traffic_volume` Numeric Hourly I-94 ATR 301 reported westbound traffic volume

## Summary of Findings
The analysis revealed that time is a significant traffic indicator, with clear patterns observed:

* Heavy traffic tends to occur during the warmer months, spanning from March to October.
* Traffic volume is higher on weekdays compared to weekends, aligning with typical commuting patterns.
* Weekdays witness peak rush hours around 7 AM and 4 PM, showing periods of intensified traffic.
* Weather conditions also play a role, with traffic volume decreasing during adverse weather conditions.

## Predicting Traffic Volume
Following the exploratory data analysis of the hourly traffic volume on the westbound I-94 in Minneapolis-St Paul, MN, I proceeded to build a model to predict the hourly traffic volume from relevant features.

* I first built a baseline regression model using linear regression. The root mean squared error (RMSE) of the baseline linear regression model, when evaluated on the test data, is 873.97.
* Subsequently, I developed a better model using Random Forest regression with an RMSE of 777.04 on the test data. 
* Compared to the baseline linear regression model, the Random Forest model achieved a lower RMSE, implying that it provides more accurate predictions on average.