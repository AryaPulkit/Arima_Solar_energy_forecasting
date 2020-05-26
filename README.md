# Arima_Solar_energy_forecasting

#Problem Statement:

To predict the generation of power of the given plan in this duration:
October 1st, 2019 to October 27th, 2019.

#Data Preprocessing and Feature Engineering:

The data contains 70080 rows and 5 features. To proceed ahead we need to convert the datetime to datetime64 format. Then I looked for missing values and decided to drop the two features ghi and gti as the majority of the data was missing as imputation was not feasible. Then we group the data based on the date and set the date as the index.

#Exploratory Data Analysis: 

Initially, we plotted scatter plot , histogram and box plot and found out that the data was containing outliers which need to be processed and we imputed the outliers with the median values. Moving ahead we check whether the data was stationary or not using Augmented Dickey-Fuller test.

#Model Building and Model Evaluation:

We used statsmodel library to build the model using ARIMA. We Build the model using log values of the power and plotted sum of square residuals. then we predicted the values and forecasted the values with 95% Confidence Interval.
