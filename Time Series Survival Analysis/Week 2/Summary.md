Summary/Review
Stationarity
Stationarity impacts our ability to model and forecast

A stationary series has the same mean and variance over time

Non-stationary series are much harder to model

Common approach:

Identify sources of non-stationarity

Transform series to make it stationary

Build models with stationary series

The Augmented Dickey-Fuller (ADF) test specifically tests for stationarity.

It is a hypothesis test: the test returns a p-value,  and we generally say the series is non-stationary if the p-value is less than 0.05.

It is a less appropriate test to use with small datasets,  or data with heteroscedasticity (different variance across observations) present.

It is best to pair ADF with other techniques such as:  run-sequence plots, summary statistics, or histograms.

Common Transformations for Time Series include:

Transformations allow us to generate stationary inputs required by most models.

There are several ways to transform nonstationary time series data:

Remove trend (constant mean)

Remove heteroscedasticity with log (constant variance)

Remove autocorrelation with differencing (exploit constant structure)

Remove seasonality (no periodic component)

Multiple transformations are often required.

Time Series Smoothing
Smoothing is a process that often improves our ability to forecast series by reducing the impact of noise.

There are many ways to smooth data. Some examples:

Simple average smoothing

Equally weighted moving average

Exponentially weighted moving average

This are some suggestions for selecting a Smoothing Technique. If your data:

–       lack a trend
Then use Single Exponential Smoothing

–       have trend but no seasonality
Then use Double Exponential Smoothing

–       have trend and seasonality
Then use Triple Exponential Smoothing