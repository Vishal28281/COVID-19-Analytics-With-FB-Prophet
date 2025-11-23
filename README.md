# COVID-19 Data Analysis & Forecasting

This project analyses the global spread of COVID-19 using Python, Pandas, and Facebook Prophet.  
It covers data cleaning, exploratory data analysis (EDA), visualisation, and time-series forecasting of confirmed cases, recoveries, and deaths.

---

## 📌 Project Overview

The objective of this project is to understand COVID-19 trends and predict future case counts using historical data. The analysis includes:

- Importing and preprocessing global COVID-19 datasets  
- Performing exploratory data analysis (EDA)
- Visualising trends across countries
- Identifying patterns in confirmed, recovered, and death cases
- Building a forecasting model using **FB Prophet**
- Generating predictions for future COVID-19 cases

---

## 📂 Dataset

The dataset used in this project:

- **File:** `covid_19_clean_complete.csv`
- **Source:** Kaggle / public COVID-19 global time-series data  
- **Columns Include:**  
  - *Date (ds)*  
  - *Confirmed*  
  - *Recovered*  
  - *Deaths*  
  - *Country/Region*  
  - *Province/State*  
  - *Active cases*  

---

## 🛠️ Tools & Libraries Used

- **Python**
- **Pandas** – data manipulation
- **NumPy** – numerical operations
- **Matplotlib** – visualizations
- **FB Prophet** – forecasting model

---

## 📊 Key Steps in the Project

### 1. **Data Import**
```python
df = pd.read_csv("covid_19_clean_complete.csv")

### 2. Data Exploration

Checking data types

Listing unique countries

Understanding missing values

3. Visualisation

Line charts of confirmed, recovered & death trends

Country-wise comparisons

Daily progression curves

4. Prophet Forecasting

The dataset is prepared for Prophet:

# Prophet requires 'ds' and 'y columns
# ds = date
# y = target variable (confirmed cases)


The model is then trained to generate:

Future predictions

Trend graphs

Components such as weekly & yearly patterns

📈 Forecasting Output

The model generates:

Future COVID-19 case predictions

Trend analysis

Seasonal components

These insights help understand how COVID-19 might progress based on historical behaviour.

📦 How to Run the Project

Install required libraries:

pip install pandas numpy matplotlib prophet


Open the notebook:

jupyter notebook Covid_19_Project.ipynb


Run all cells sequentially.

📑 Project Structure
├── Covid_19_Project.ipynb     # Main analysis notebook
├── covid_19_clean_complete.csv # Dataset
└── README.md                   # Project documentation

🙌 Acknowledgements

COVID-19 dataset providers

Prophet forecasting library from Meta (Facebook)

Open-source Python data science ecosystem

