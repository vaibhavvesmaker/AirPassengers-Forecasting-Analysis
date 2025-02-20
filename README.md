# **AirPassengers Forecasting Analysis**

## **Project Overview**
This project performs a time series forecasting analysis on the **AirPassengers** dataset, a built-in dataset in R that contains monthly totals of international airline passengers from **1949 to 1960**. The goal is to analyze trends, seasonality, and make future predictions using statistical forecasting methods.

## **Dataset**
- **Name**: AirPassengers
- **Description**: Monthly airline passenger counts from 1949 to 1960.
- **Number of Observations**: 144 (12 years of monthly data).
- **Variables**: 
  - **Month** (Time index)
  - **Passengers** (Number of airline passengers in thousands)

## **Analysis Steps**
### 1. **Exploratory Data Analysis (EDA)**
- Visualized the time series data to observe **trends** and **seasonality**.
- Examined the **distribution** and **seasonal decomposition** of the series.

### 2. **Data Preprocessing**
- Converted the dataset into a **time series object** in R.
- Checked for **missing values** and performed **log transformation** to stabilize variance.

### 3. **Time Series Decomposition**
- Used **classical decomposition** to separate the series into:
  - **Trend** (Long-term movement)
  - **Seasonality** (Yearly repeating patterns)
  - **Residuals** (Random fluctuations)

### 4. **Forecasting Methods**
- Applied **Auto-Regressive Integrated Moving Average (ARIMA)** modeling.
- Used the **Holt-Winters method** for seasonal adjustment.
- Selected the best model using **Akaike Information Criterion (AIC)**.
- Generated **future forecasts** for the next few years.

### 5. **Model Evaluation**
- Compared different models based on **Mean Absolute Error (MAE)** and **Root Mean Squared Error (RMSE)**.
- Validated the model using **train-test split**.

## **Results and Insights**
- **Passenger numbers exhibited an increasing trend over time.**
- **Clear seasonal patterns** were observed, with peaks in summer months.
- **ARIMA(0,1,1)(0,1,1)[12]** was selected as the best model for forecasting.
- The **forecast predicts continued growth** in passenger numbers.

## **Technologies Used**
- **R programming**
- **ggplot2** (for data visualization)
- **forecast** package (for ARIMA and Holt-Winters models)
- **tseries** package (for stationarity testing)

## **Usage**
To run the analysis, execute the R script or RMarkdown file. The script will:
1. Load the dataset.
2. Perform time series decomposition.
3. Apply and evaluate forecasting models.
4. Generate future predictions.

## **Future Enhancements**
- Incorporate **Deep Learning** models (e.g., LSTMs) for improved forecasting.
- Apply **external regressors** (economic indicators, fuel prices) for better model accuracy.
- Develop an **interactive dashboard** using Shiny in R.

