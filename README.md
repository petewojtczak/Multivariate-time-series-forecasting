**Weather Forecasting with sktime**<br>

Weather forecasting is widely recognized as a notoriously challenging task. This notebook aims to demonstrate the implementation of sktime algorithm (specifically VAR) rather than focusing on creating a highly accurate weather forecast model (although a simple prediction is provided). Some interesting preprocessing steps are applied: a second-degree polynomial detrender, z-score normalization to remove arbitrary units, followed by VAR estimation. Extensive post-estimation testing reveals that the residuals are not normally distributed and exhibit heteroscedasticity.

<br>**What is VAR?**<br>

VAR (Vector Autoregression) is a classic multivariate linear model that has been extensively researched for decades. The model assumes that each variable depends linearly on its own lagged values and the lagged values of all other variables in the system. It is widely used in econometrics and time series analysis. However, its effectiveness depends on whether its underlying assumptions are met, such as stationarity of the time series and absence of serial correlation in the residuals. When these assumptions hold true, VAR can be a very powerful tool for modeling and forecasting multivariate time series data.

<br>**What is sktime?**<br>

Sktime is an open-source Python library specifically designed for time series analysis and forecasting tasks. It provides a user-friendly interface similar to sklearn (scikit-learn) and integrates seamlessly with it. sktime is particularly useful for applying sklearn machine learning algorithms to time series forecasting tasks, including gridsearching them.
<br>
Data source: https://www.kaggle.com/datasets/swatikhedekar/python-project-on-weather-dataset
