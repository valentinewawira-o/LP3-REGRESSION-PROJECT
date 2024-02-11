# LP3-REGRESSION-PROJECT
Prediction of store sales on data from Corporation Favorita, a large Ecuadorian-based grocery retailer
his project aims to create a robust time series forecasting model that accurately predicts unit sales for various items sold in Favorita stores. Favorita, a prominent grocery retailer in Ecuador, provides the sales data for this model. The dataset encompasses sales information for numerous items across different stores, presenting a complex and challenging problem.To construct a precise forecasting model, a combination of statistical and machine learning techniques will be employed. The data will undergo preprocessing to ensure cleanliness, consistency, and suitability for analysis. Exploratory Data Analysis (EDA) techniques will be utilized to gain a comprehensive understanding of the data, identifying patterns and trends within the sales information. 
The fully colored seasonal component indicates prominent recurring patterns at fixed intervals, likely due to seasonal factors influencing sales. The residual component shows mostly random behavior, but with a few outliers suggesting some patterns yet to be fully captured by the model.

The ADF test is commonly used to determine the stationarity of a time series. Stationarity is an important concept in time series analysis, as it ensures that the statistical properties of the series remain constant over time. A stationary time series exhibits a constant mean, variance, and autocovariance structure, making it easier to model and forecast.By performing the ADF test and checking the p-value, we can assess whether the 'sales' data in the 'train_df' DataFrame is stationary or not. If the p-value is below the chosen significance level (0.05 in this case), you can conclude that the time series is stationary, indicating that it has a stable mean and variance over time.
The results obtained from the forecasting models will be scrutinized, and the insights derived will guide informed business decisions. These insights may include recognizing products with high demand during specific periods, identifying store performance variations, and detecting trends in sales data that can inform marketing and inventory strategies.


Several time series forecasting models will be deployed to forecast store sales, including ARIMA, Linear Regression, and others. These models will be trained using historical sales data, and their accuracy will be assessed using various performance metrics such as root mean square logarithmic error, root mean squared error (RMSE), and mean square error (MSE).
We are training four different models and evaluating their performance using mean absolute error (MAE) and root mean squared error (RMSE). Here's an overview of the steps involved in the process:

ARIMA: We initialize and fit the ARIMA model, which is a classical time series forecasting model. ARIMA can capture autoregressive and moving average components in the data.

SARIMA: We initialize and fit the SARIMA model, which extends ARIMA to include seasonal components. SARIMA is suitable for capturing seasonal patterns in the data along with autoregressive and moving average components.

XGBoost Regressor: We initialize and fit the XGBoost Regressor model. XGBoost is a gradient boosting algorithm known for its speed and performance. It can handle both numerical and categorical features and is effective in capturing complex relationships in the data.

CatBoost Regressor: We initialize and fit the CatBoost Regressor model. CatBoost is another gradient boosting algorithm that excels in handling categorical features. It automatically handles categorical variables and provides accurate predictions with minimal data preprocessing.


After training these models, we evaluate their performance by making predictions on the test data and calculating the MAE and RMSE. Lower values of MAE and RMSE indicate better predictive accuracy


By performing the ADF test and checking the p-value, we can assess whether the 'sales' data in the 'train_df' DataFrame is stationary or not. If the p-value is below the chosen significance level (0.05 in this case), you can conclude that the time series is stationary, indicating that it has a stable mean and variance over time.
The results obtained from the forecasting models will be scrutinized, and the insights derived will guide informed business decisions. These insights may include recognizing products with high demand during specific periods, identifying store performance variations, and detecting trends in sales data that can inform marketing and inventory strategies.

In summary, the project’s overarching objective is to establish a dependable time series forecasting model that can assist Favorita in optimizing sales strategies and enhancing overall profitability