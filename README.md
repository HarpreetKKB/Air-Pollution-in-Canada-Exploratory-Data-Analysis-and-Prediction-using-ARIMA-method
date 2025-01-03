# Air-Pollution-in-Canada-Exploratory-Data-Analysis-and-Prediction-using-ARIMA-method

# Air Pollution Analysis and Forecasting

## Overview
Air pollution is a major global environmental risk, adversely affecting human health and food security. It involves the release of pollutants into the atmosphere that harm both people and the planet. Policies aimed at reducing air pollution can serve as a dual-benefit strategy by improving public health and mitigating climate change.

Accurate air pollutant forecasting is essential to minimizing the impact of pollution peaks on populations and ecosystems. This work focuses on forecasting air pollutant levels to enable timely measures to reduce high pollutant concentrations.

---

## Objective
The objectives of this project are:

1. **Exploration of Trends**: Analyze air pollutant emissions from various provinces in Canada using time series analysis to provide a comprehensive overview of trends over time.
2. **Pollutant Level Forecasting**: Predict pollutant levels in the province with the highest emissions using the ARIMA model.
3. **Source Contribution Analysis**: Identify and analyze the primary sources responsible for high pollutant levels in each province.

---

## Data Source

The data for this project is sourced from the open data platform of **Canada's Air Pollutant Emissions Inventory - Environment and Climate Change Canada Data**.

- **Data File**: `EN_APEI-Can-Prov_Terr.csv`
- **Attributes Studied**:
  - Total Particulate Matter (TPM)
  - Particulate Matter ≤ 10 microns (PM10)
  - Particulate Matter ≤ 2.5 microns (PM2.5)
  - Sulphur Oxides (SOx)
  - Nitrogen Oxides (NOx)
  - Carbon Monoxide (CO)

---

## Analysis

### Data Pre-processing
The data pre-processing stage involved:
- Handling missing values (e.g., filling NaN values with mean values or removing them).
- Removing or altering outliers to improve data quality.
- Selecting relevant columns focused on key pollutants for further analysis.

### Exploratory Data Analysis (EDA)
EDA was performed to:
- Understand the statistical properties of the dataset.
- Visualize trends and patterns in pollutant emissions.

### Forecasting with ARIMA
- The ARIMA model was used for time series forecasting of pollutant levels.
- Optimization of model parameters (‘p’, ‘d’, ‘q’) was performed, with values set to 1, 1, and 2, respectively.

---

## Challenges Faced

1. **Large Dataset**:
   - The dataset was extensive, requiring a subset to be selected for analysis.
   - Missing values were filled or removed to ensure data integrity.

2. **Units of Measurement**:
   - Pollutant data was in tonnes per year, making it impossible to estimate the Air Quality Index (AQI) for provinces.
   - Efforts to find authenticated AQI records were unsuccessful, leading to the use of ARIMA for forecasting.

3. **ARIMA Optimization**:
   - The optimization of `p`, `d`, and `q` parameters was challenging.
   - A thorough understanding of time series analysis was necessary before implementing the ARIMA model.

---

## Conclusion
This work provides insights into the trends and sources of air pollution in Canada, focusing on forecasting pollutant levels using ARIMA. The findings might assist in implementing timely measures to reduce air pollution and its adverse effects.

---

## Usage
To replicate this project or explore the analysis further, you can:
- Download the dataset from Canada's Air Pollutant Emissions Inventory.
- Use the provided ARIMA configuration for forecasting pollutant levels.
- Modify the analysis to focus on specific pollutants or regions.

---

## Disclaimer
This project is intended for educational learning and research purposes only. The data and analyses provided in this repository are based on publicly available sources and involve certain assumptions and limitations. 

While every effort has been made to ensure accuracy, the predictions and insights generated by the ARIMA model are subject to variability and should not be used as a sole basis for decision-making. The findings should be considered indicative rather than definitive.

The author is not responsible for any actions taken based on the information in this work. This work is intented for learning python language for data analysis only. 

