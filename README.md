# 🌡️ Time Series Forecasting: Daily Minimum Temperature Prediction

An end-to-end machine learning project that forecasts daily minimum temperatures using statistical, machine learning, and deep learning models. This project analyzes 10 years of temperature data and compares multiple forecasting approaches to identify the most effective model.

## 📊 Dataset

- **Location:** Melbourne, Australia
- **Period:** 1981–1990
- **Records:** 3,650 daily observations
- **Target Variable:** Daily Minimum Temperature (°C)

## 🚀 Project Workflow

### 🔍 Exploratory Data Analysis
- Descriptive statistics and trend analysis
- Seasonal decomposition
- Temperature heatmaps and visualizations
- Correlation analysis

### ⚙️ Data Preprocessing & Feature Engineering
- Missing value verification
- Outlier detection (IQR & Z-Score)
- Feature scaling with StandardScaler
- Time-based feature creation:
  - Month
  - Year
  - Day of Week
  - Season
  - Lag Features (1-day and 7-day)

### 🤖 Model Development
The following forecasting models were trained and evaluated:

- Linear Regression
- Random Forest Regressor
- ARIMA (7,0,0)
- LSTM Neural Network

## 📈 Model Performance

| Model | MAE | R² Score |
|---------|---------|---------|
| Linear Regression | 0.4485 | 0.6452 |
| Random Forest (Tuned) | 0.4669 | 0.6197 |
| ARIMA | 0.8270 | -0.0859 |
| LSTM | **0.2183** | **0.9121** |

### Key Findings
- Lag features were the strongest predictors.
- Linear Regression delivered strong performance with low complexity.
- Random Forest captured non-linear relationships but offered limited improvement.
- ARIMA underperformed due to parameter limitations.
- LSTM achieved the best forecasting accuracy and overall performance.

## 💡 Business Applications

- Energy demand forecasting
- Grid load balancing
- Agricultural planning
- Predictive maintenance
- Weather-driven inventory optimization

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- TensorFlow / Keras
- Google Colab

## 📂 Project Structure

```text
Time-Series-Temperature-Forecasting/
│
├──Time-Series-Forecasting-Presantation.pdf        #Presentation
│
├──Time-Series-Forecasting-Project.pdf             #PDF
│
├── data/
│   └── daily-minimum-temperatures.csv
│
├── Google Colab/
│   └── Time_Series_Forecasting.ipynb
└── README.md
