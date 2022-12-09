# Modeling Japan's Activity Rate in the 21st Century

Final Project for PSTAT 174: Time Series

## Abstract

In this paper, we investigate the monthly activity rates of Japanese people ages 25-54 for the years 2000-2021. The activity rate is the percentage of the civilian non-institutional population that is either employed or actively looking for a job.

We seek to identify an appropriate time series model for this data using the Box-Jenkins methodology. We first try a Box-Cox transformation on the original time series data (from January 2000 to December 2020) to stabilize the variance, though the transformation does not significantly change its overall shape. Since the data exhibits a positive linear trend and seasonality, we difference once at both lags 1 and 12, respectively. We then identify several potential models using the ACF and PACF plots of the differenced series and choose a $\text{SARIMA}(0, 1, 2) \times (0, 1, 7)_{12}$ model with 4 parameters for the original data based on the lowest AICC. After running some diagnostic tests to ensure that the residuals of this model are Gaussian white noise, we use our model to forecast the activity rates for the months between January 2021 and December 2021. Although one prediction fell outside of the prediction interval, the model does an adequate job at forecasting.
