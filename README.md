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
time-series-temperature-forecasting/
│
├── data/
│   └── daily-minimum-temperatures.csv
│
├── notebooks/
│   └── Time_Series_Forecasting.ipynb
│
├── images/
│   ├── seasonal_decomposition.png
│   ├── heatmap.png
│   ├── correlation_matrix.png
│   └── model_comparison.png
│
└── README.md
```

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/your-username/time-series-temperature-forecasting.git
cd time-series-temperature-forecasting
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels tensorflow
```

### Run the Notebook

```bash
jupyter notebook Time_Series_Forecasting.ipynb
```

## 👤 Author

**Arif Hussain Syed**

Master's Student in Data Analytics

## 📄 License

This project is licensed under the MIT License.
