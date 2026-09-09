# 🌾 Seasonal Agriculture Performance Analysis

## 📌 Project Overview

**Seasonal Agriculture Performance Analysis** is a data analysis project that investigates how agricultural performance varies across different seasons.

The project analyzes agricultural, environmental, resource usage, and economic factors to identify meaningful **seasonal patterns, relationships, variations, and unusual observations**.

The analysis focuses on comparing **Kharif, Rabi, and Zaid** seasons using data related to crop yield, production, rainfall, temperature, soil conditions, irrigation, water usage, costs, revenue, profit, and disease/pest risk.

---

## 🎯 Problem Statement

Agricultural performance can vary significantly depending on seasonal environmental conditions, farming practices, resource availability, and economic factors.

This project aims to analyze the dataset and answer questions such as:

* How does agricultural performance vary across seasons?
* What major seasonal patterns can be observed?
* Which agricultural characteristics change between seasons?
* How does resource usage vary across seasons?
* Are environmental conditions related to agricultural performance?
* How do revenue, cost, and profit vary across seasons?
* Are there unusual or unexpected seasonal patterns?
* How can the findings support better seasonal agricultural planning?

---

## 🎯 Objectives

The main objectives of this project are:

* Explore and understand the agricultural dataset.
* Clean and prepare the data for analysis.
* Compare agricultural performance across seasons.
* Identify important seasonal patterns and trends.
* Analyze relationships between environmental conditions and crop performance.
* Compare resource usage and irrigation methods.
* Analyze economic performance across seasons.
* Identify unusual patterns and variations.
* Create meaningful visualizations.
* Develop evidence-based conclusions and recommendations.

---

## 📊 Dataset

The dataset contains **4,000 agricultural records** and **28 columns**.

### Important Features

| Category              | Features                                  |
| --------------------- | ----------------------------------------- |
| Farm Information      | Farm ID, State, District                  |
| Crop Information      | Crop, Season                              |
| Farm Characteristics  | Farm Area                                 |
| Environmental Factors | Rainfall, Temperature, Humidity, Sunlight |
| Soil Conditions       | Soil pH, Soil Moisture                    |
| Nutrients             | Nitrogen, Phosphorus, Potassium           |
| Farming Practices     | Irrigation Method, Fertilizer, Pesticide  |
| Crop Quality          | Seed Quality Score                        |
| Performance           | Yield, Production                         |
| Economic Factors      | Market Price, Cost, Revenue, Profit       |
| Resource Usage        | Water Used, Water Efficiency              |
| Risk                  | Disease/Pest Risk                         |

---

## 🛠️ Technologies Used

This project uses only the following Python libraries:

* **NumPy** – Numerical calculations
* **Pandas** – Data loading, cleaning, manipulation and analysis
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization

### Tools

* Python
* Jupyter Notebook
* Git & GitHub

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the CSV dataset using Pandas.
2. Inspected the dataset structure and data types.
3. Checked for missing values.
4. Identified missing values in:

   * `Rainfall_mm`
   * `Soil_Moisture_pct`
   * `Yield_Tonnes_Ha`
5. Missing numerical values were handled using median imputation.
6. Checked for duplicate records.
7. Verified numerical and categorical columns before analysis.

---

## 📈 Analysis Performed

### 1. Seasonal Distribution

The number of records belonging to each season was analyzed.

* Kharif: **1,779**
* Rabi: **1,627**
* Zaid: **594**

### 2. Seasonal Performance

Yield, production, revenue, cost, profit and water efficiency were compared across seasons.

### 3. Environmental Analysis

The following environmental factors were analyzed:

* Rainfall
* Average temperature
* Humidity
* Soil moisture
* Sunlight

### 4. Resource Usage

The project analyzes:

* Water usage
* Water efficiency
* Fertilizer usage
* Pesticide usage
* Irrigation methods

### 5. Economic Analysis

Economic performance was evaluated using:

* Market price
* Total cost
* Revenue
* Profit
* Profit/Loss status

### 6. Crop Analysis

Crop-level performance was compared across different crops and seasons.

### 7. Correlation Analysis

Relationships between important numerical variables were investigated using correlation analysis and heatmaps.

### 8. Outlier Analysis

The IQR method was used to identify potential outliers in important numerical variables.

---

# 🔍 Key Findings

## 🌧️ 1. Kharif showed the strongest overall performance

Kharif recorded the highest average:

* Yield: **~5.63 tonnes/ha**
* Production: **~46.31 tonnes/farm**
* Revenue: **~₹7.11 lakh/farm**
* Profit: **~₹1.79 lakh/farm**
* Water efficiency: **~5.89 tonnes/1000 m³**

Kharif also had the highest rainfall, humidity and soil moisture.

---

## 🌾 2. Rabi showed moderate performance

Rabi recorded:

* Average yield: **~5.04 tonnes/ha**
* Average production: **~41.49 tonnes/farm**
* Average profit: **~₹87,689/farm**

Its performance was generally between Kharif and Zaid.

---

## ☀️ 3. Zaid showed the weakest economic performance

Zaid recorded:

* Average yield: **~4.64 tonnes/ha**
* Average production: **~38.89 tonnes/farm**
* Average revenue: **~₹5.19 lakh/farm**
* Average profit: **~−₹24,805/farm**
* Average water efficiency: **~4.41 tonnes/1000 m³**

Zaid was the only season with a negative average profit.

---

## 💧 4. Zaid used the most water

Average water usage:

| Season | Water Used |
| ------ | ---------: |
| Kharif |  ~6,102 m³ |
| Rabi   |  ~5,847 m³ |
| Zaid   |  ~6,420 m³ |

Zaid therefore had both **high water usage and low water efficiency**, making water management an important concern.

---

## 🌧️ 5. Rainfall alone did not strongly explain yield

The overall correlation between rainfall and yield was approximately:

**0.03**

This indicates a very weak overall linear relationship between rainfall and yield in this dataset.

Therefore, agricultural performance appears to depend on multiple factors rather than rainfall alone.

---

## 🚜 6. Irrigation method affected performance

Average yield by irrigation method:

| Irrigation Method |   Average Yield |
| ----------------- | --------------: |
| Drip              | ~6.58 tonnes/ha |
| Sprinkler         | ~5.16 tonnes/ha |
| Flood             | ~4.86 tonnes/ha |
| Rainfed           | ~4.60 tonnes/ha |

Drip irrigation recorded the highest average yield among the irrigation methods in this dataset.

---

## 💦 7. Rainfed farming showed high water efficiency

Average water efficiency:

| Irrigation Method | Water Efficiency |
| ----------------- | ---------------: |
| Rainfed           |            ~7.56 |
| Drip              |            ~6.27 |
| Sprinkler         |            ~4.67 |
| Flood             |            ~3.44 |

This result should be interpreted carefully because water efficiency and total water availability are different measures.

---

## 🐛 8. Kharif had the highest disease/pest risk

Average disease/pest risk:

* Kharif: **~54.47%**
* Rabi: **~40.48%**
* Zaid: **~38.22%**

Despite having the highest disease/pest risk, Kharif also achieved the strongest overall performance.

---

## 📊 9. Yield had a strong relationship with water efficiency

The correlation between yield and water efficiency was approximately:

**0.915**

Yield also showed strong positive relationships with production and moderate positive relationships with revenue and profit.

> Correlation indicates association and does not necessarily prove causation.

---

## 🌱 10. Sugarcane had the highest yield

Among the crops in the dataset, sugarcane recorded the highest average yield at approximately:

**46.64 tonnes/ha**

However, crop yields should be compared carefully because different crops naturally have different yield scales.

---

# 💡 Conclusions

The analysis shows that agricultural performance varies considerably across seasons.

**Kharif performed the strongest overall**, with higher yield, production, revenue, profit and water efficiency. However, it also experienced higher disease/pest risk.

**Rabi showed moderate performance**, while **Zaid showed the weakest economic performance**, including negative average profit and relatively low water efficiency.

The analysis also indicates that environmental factors alone cannot fully explain agricultural performance. Rainfall had almost no overall linear correlation with yield, suggesting that factors such as irrigation, soil conditions, crop type, farming practices, resource usage and economic conditions may all contribute to the observed outcomes.

Overall, the results demonstrate the importance of **season-specific agricultural planning and efficient resource management**.

---

# 📌 Recommendations

Based on the analysis, the following recommendations can be considered:

### 1. Improve Zaid-season planning

Zaid showed negative average profit and low water efficiency. Farmers should carefully evaluate crop selection, input costs and expected market returns before cultivation.

### 2. Improve water management

Since Zaid used the highest amount of water while having the lowest water efficiency, better irrigation scheduling and water-management practices should be considered.

### 3. Consider efficient irrigation methods

Drip irrigation showed the highest average yield in the dataset. It can be considered where it is economically and technically suitable.

### 4. Strengthen Kharif pest management

Kharif showed the highest disease/pest risk. Early monitoring and preventive pest-management strategies can help reduce potential losses.

### 5. Avoid relying only on rainfall

Since rainfall had a very weak overall correlation with yield, agricultural planning should consider multiple factors rather than rainfall alone.

### 6. Consider crop-specific planning

Different crops have very different yield levels and requirements. Crop selection should consider season, soil, water availability, expected yield, market price and production costs.

### 7. Monitor water efficiency

Water efficiency should be tracked along with yield and production to identify farming practices that achieve better output with available water resources.

### 8. Control input costs

The negative average profit observed in Zaid indicates the importance of carefully managing fertilizer, pesticide, irrigation and other production costs.

---

# 📂 Project Structure

```text
Seasonal-Agriculture-Performance-Analysis/
│
├── data/
│   └── seasonal_agriculture_performance_dataset.csv
│
├── notebooks/
│   └── Seasonal_Agriculture_Performance_Analysis.ipynb
│
├── images/
│   ├── seasonal_distribution.png
│   ├── seasonal_yield.png
│   ├── seasonal_profit.png
│   ├── water_efficiency.png
│   ├── irrigation_yield.png
│   └── correlation_heatmap.png
│
├── README.md
└── requirements.txt
```

---

# ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Seasonal-Agriculture-Performance-Analysis.git
```

### 2. Navigate to the project folder

```bash
cd Seasonal-Agriculture-Performance-Analysis
```

### 3. Install the required libraries

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the notebook

Open:

```text
notebooks/Seasonal_Agriculture_Performance_Analysis.ipynb
```

Run the cells from top to bottom.

---

# 📊 Visualizations

The project includes visualizations such as:

* Seasonal distribution

  
  <img width="698" height="463" alt="image" src="https://github.com/user-attachments/assets/1bf86655-5d0d-48e9-b5c6-352e61be4922" />

* Average yield by season

  
  <img width="672" height="466" alt="image" src="https://github.com/user-attachments/assets/34484022-6eb6-4b4c-976e-12bf06a508ff" />

* Total production by season


  <img width="712" height="467" alt="image" src="https://github.com/user-attachments/assets/0e0789e9-b397-491e-be18-6cfbf88b1e38" />

* Rainfall distribution


  <img width="701" height="465" alt="image" src="https://github.com/user-attachments/assets/81be83e4-8f21-41c9-b76e-f05a563f230b" />

* Rainfall vs. yield


  <img width="770" height="542" alt="image" src="https://github.com/user-attachments/assets/92263ef6-36d0-4bbf-8e2c-547091f5db7d" />

* Temperature vs. yield


  <img width="770" height="543" alt="image" src="https://github.com/user-attachments/assets/ccd0faae-00e4-4c64-9663-74c486f386e2" />

* Soil moisture vs. yield


  <img width="767" height="541" alt="image" src="https://github.com/user-attachments/assets/a0cdc67c-1533-41d1-8bdc-fdff01920e75" />

* Water usage comparison


  <img width="701" height="465" alt="image" src="https://github.com/user-attachments/assets/3f823793-3b40-4292-a727-7d6086d8bcf3" />

* Water efficiency comparison


  <img width="671" height="463" alt="image" src="https://github.com/user-attachments/assets/fcd5ae95-ee9d-456c-b622-3398c50076e9" />

* Irrigation vs. yield


  <img width="752" height="463" alt="image" src="https://github.com/user-attachments/assets/4882cd43-8c0e-4ff3-ab73-73a11f5c6b35" />

* Crop yield comparison


  <img width="842" height="592" alt="image" src="https://github.com/user-attachments/assets/5b049b24-448f-421b-be29-38688b1fb54e" />

* Disease/pest risk analysis


  <img width="682" height="462" alt="image" src="https://github.com/user-attachments/assets/b102b83a-917a-4162-a485-702823ea83e6" />
  <img width="770" height="537" alt="image" src="https://github.com/user-attachments/assets/8a388858-096a-46ca-bd82-128d46a77a33" />

* State-wise performance


  <img width="817" height="557" alt="image" src="https://github.com/user-attachments/assets/c4798211-9a52-4234-8ec8-425b3f2d6b86" />

* Correlation heatmap


  <img width="775" height="557" alt="image" src="https://github.com/user-attachments/assets/269fb132-4bd0-4637-8659-352e315bd3c0" />

* Outlier analysis


  <img width="622" height="422" alt="image" src="https://github.com/user-attachments/assets/057a01bd-0004-4c0c-9e85-d17711fcb10d" />


---

# 🚀 Future Improvements

Possible future improvements include:

* Developing an interactive dashboard.
* Adding more years of agricultural data.
* Including additional weather variables.
* Building predictive models for crop yield.
* Developing crop recommendation systems.
* Forecasting seasonal profitability.
* Performing more detailed regional analysis.
* Adding real-time weather and market-price information.

---

# 👨‍💻 Author

**Devi Sri Surya Sankar Chollangi**

### Project

**Seasonal Agriculture Performance Analysis**

### Technologies

Python | NumPy | Pandas | Matplotlib | Seaborn

---

## ⭐ Project Highlights

* 📊 4,000 agricultural records
* 🌾 3 major seasons analyzed
* 🌱 Multiple crops and regions
* 💧 Water and irrigation analysis
* 💰 Revenue, cost and profit analysis
* 🌦️ Environmental analysis
* 🐛 Disease/pest risk analysis
* 📈 Correlation and outlier analysis
* 📉 Extensive data visualizations

---

## 📜 License

This project is intended for **educational and academic purposes**.
