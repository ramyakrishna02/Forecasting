# Forecasting
Time series forecasting is the process of fitting a model to time-stamped, historical data to predict future values. It is an important machine learning analysis method with various use-cases, such as predicting the electricity consumption from the smart meters that can help the Electricity company plan the network expansion.

In time series forecasting, we fit a model to time-stamped historical data to predict future values. For example, we can predict the demand for a product in the next ten months based on historical data of five years. 

Machine learning forecasting is a process that uses algorithms to learn from data and make predictions about future events. It can be used to understand audience needs or predict trends.

## Implementation
- Importing the required Libraries and reading the dataset
- Performing EDA on the data
- Feature Engineer
- Visualizations
- Moving Average
  - Time series decomposition plot
  - Autocorrelation Plot (ACF)
  - Partial Autocorrelation Plot (PACF)
- Data Preprocessing
- Splitting the data into Train and Test data
- Choosing the Evaluation Metrics - RMSE & MAPE
- Building the Models
  - Linear Model, Exponential Model, Quadratic Model
  - Exponential Smoothing
    - Simple Exponential, Holt Method, Holts Winter Exponential Smoothing
  - Seasonalities
    - Additive, Additive with quadratic trend, Multiplicative, Multiplicative Additive Seasonality
  - ARIMA Model
- Conclusion
  - Comparing all the created models
  - Finalized Model

## Packages Used
- pandas, numpy
- matplotlib.pyplot, seaborn
- warnings
- from pandas import Grouper
- from pandas.plotting import lag_plot
- from statsmodels.graphics.tsaplots import plot_acf
- from statsmodels.graphics.tsaplots import plot_pacf
- import statsmodels.formula.api as smf
- from statsmodels.tsa.seasonal import seasonal_decompose
- from statsmodels.tsa.holtwinters import SimpleExpSmoothing
- from statsmodels.tsa.holtwinters import Holt
- from statsmodels.tsa.holtwinters import ExponentialSmoothing
- from sklearn.metrics import mean_squared_error
- from statsmodels.tsa.arima.model import ARIMA
- from statsmodels.tsa.stattools import adfuller
