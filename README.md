🌡️ Time Series Forecasting: Daily Minimum Temperature Prediction

An end-to-end machine learning project that forecasts daily minimum temperatures using statistical, machine learning, and deep learning models. The project analyzes 10 years of temperature data and compares multiple forecasting approaches to identify the most effective model.

📊 Dataset

* Location: Melbourne, Australia
* Period: 1981–1990
* Records: 3,650 daily observations
* Target Variable: Daily Minimum Temperature (°C)

🚀 Project Workflow

1. Exploratory Data Analysis

* Descriptive statistics and trend analysis
* Seasonal decomposition
* Temperature heatmaps and visualizations
* Correlation analysis

2. Data Preprocessing & Feature Engineering

* Missing value verification
* Outlier detection (IQR & Z-Score)
* Feature scaling with StandardScaler
* Time-based features:
    * Month
    * Year
    * Day of Week
    * Season
    * Lag Features (1-day and 7-day)

3. Model Development

The following forecasting models were trained and evaluated:

* Linear Regression
* Random Forest Regressor
* ARIMA (7,0,0)
* LSTM Neural Network

📈 Model Performance

Model	MAE	R²
Linear Regression	0.4485	0.6452
Random Forest (Tuned)	0.4669	0.6197
ARIMA	0.8270	-0.0859
LSTM	0.2183	0.9121

Key Findings

* Lag features were the strongest predictors.
* Linear Regression provided strong performance with minimal complexity.
* Random Forest captured non-linear patterns but offered limited improvement.
* ARIMA underperformed due to parameter limitations.
* LSTM achieved the best forecasting accuracy, demonstrating the effectiveness of deep learning for sequential data.

🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib & Seaborn
* Scikit-learn
* Statsmodels
* TensorFlow / Keras
* Google Colab

📂 Project Structure

time-series-temperature-forecasting/
│
├── data/
├── notebooks/
├── images/
└── README.md

💡 Business Applications

* Energy demand forecasting
* Grid load balancing
* Agricultural planning
* Predictive maintenance
* Weather-driven inventory optimization

👤 Author

Arif Hussain Syed

Master’s Student in Data Analytics
