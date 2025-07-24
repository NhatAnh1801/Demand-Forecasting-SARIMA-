# Forecast time series using SARIMA model
This project demonstrates the implementation of a SARIMA (Seasonal AutoRegressive Integrated Moving Average) model to forecast product demand for a global manufacturing company. By analyzing historical data, the model aims to predict future order volumes, enabling better inventory and supply chain management.
## Dataset overview
The dataset contains historical product demand for a manufacturing company with footprints globally. The company provides thousands of products within dozens of product categories. There are four central warehouses to ship products within the region it is responsible for. Since the products are manufactured in different locations all over the world, it normally takes more than one month to ship products via ocean to different central warehouses. If forecasts for each product in different central with reasonable accuracy for the monthly demand for month after next can be achieved, it would be beneficial to the company in multiple ways.
## My workflow
My approach to this forecasting project involved the following steps:
- **Exploratory Data Analysis (EDA):** I began by conducting a thorough analysis of the original dataset to understand its structure and features.
- **Time Series Formatting and Analysis:** The data was then processed and formatted into a time series to identify trends, seasonality, and residual components.
- **Model Training and In-Sample Forecasting:** Using the insights from the analysis, I trained the SARIMA model and performed an in-sample forecast to evaluate its initial performance against historical data.
- **Model Evaluation:** The model's accuracy was assessed using standard metrics like Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and Mean Absolute Percentage Error (MAPE).
- **Out-of-Sample Forecasting:** Finally, I used the validated model to generate an out-of-sample forecast for the next five years, providing a long-term outlook on product demand.
## What I have learned
This project provided hands-on experience with several key data science and time series analysis techniques:
  - **Distribution Plotting:** Visualizing data distribution using KDE plots and QQ plots to check for skewness and normality.
  - **Data Transformation:** Applying logarithmic transformations to handle right-skewed data and stabilize variance
  - **Time Series Decomposition:** Breaking down the time series into its trend, seasonal, and residual components.
  - **Hyperparameter Tuning:** Employing a grid search to find the optimal non-seasonal (p, d, q) and seasonal (P, D, Q, s) parameters for the SARIMA model based on the Akaike Information Criterion (AIC).
  - **Forecasting Evaluation:** Measuring model performance with key metrics:
    - Root Mean Squared Error (RMSE)
    - Mean Absolute Error (MAE)
    - Mean Absolute Percentage Error (MAPE)  
## Reference
- Dataset: [Forecasts for Product Demand on Kaggle](https://www.kaggle.com/datasets/felixzhao/productdemandforecasting)
- Acknowledgements: [Forecast Order Demand and Visualization](https://www.kaggle.com/code/imsanjoykb/forecast-order-demand-and-visualization)

