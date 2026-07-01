
  
  <h1>☀️ Solar Power Generation Analysis</h1>
  
  <p>A comprehensive Data Science and Analytics project investigating the impact of environmental factors on solar energy generation.</p>

  [![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
  [![Pandas](https://img.shields.io/badge/Pandas-Data_Processing-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
  [![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/datasets/stucom/solar-energy-power-generation-dataset)
  [![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)
</div>

---

## 📑 Table of Contents
1. [Project Overview](#-project-overview)
2. [Research Questions](#-research-questions)
3. [Dataset Information](#-dataset-information)
4. [Project Objectives](#-project-objectives)
5. [Technologies Used](#-technologies-used)
6. [Project Structure](#-project-structure)
7. [Installation Guide](#-installation-guide)
8. [Data Cleaning Pipeline](#-data-cleaning-pipeline)
9. [Exploratory Data Analysis & Visualizations](#-exploratory-data-analysis--visualizations)
10. [Key Insights & Results](#-key-insights--results)
11. [Future Improvements](#-future-improvements)
12. [License & References](#-license--references)

---

## 📖 Project Overview
This project leverages **Exploratory Data Analysis (EDA)** and **Data Visualization** to understand how environmental factors such as solar radiation, temperature, and cloud cover influence solar energy generation. By building a robust data pipeline to clean and process raw telemetry data, we extract key actionable insights for renewable energy optimization.

## ❓ Research Questions
* How does solar radiation correlate with power generation?
* What is the impact of ambient temperature on the efficiency of solar panels?
* How does cloud cover dynamically affect the generated power?
* Are there underlying trends and anomalous behaviors in the power generation data?

## 📊 Dataset Information
* **Source:** [Solar Energy Power Generation Dataset (Kaggle)](https://www.kaggle.com/datasets/stucom/solar-energy-power-generation-dataset)
* **Description:** The dataset contains detailed telemetry and meteorological data including:
  * `generated_power_kw`: Power generated in Kilowatts
  * `shortwave_radiation_backwards_sfc`: Solar Radiation
  * `temperature_2_m_above_gnd`: Temperature 2 meters above ground
  * `total_cloud_cover_sfc`: Total Cloud Cover
  * `wind_speed_10_m_above_gnd`: Wind speed

## 🎯 Project Objectives
1. Perform deep data cleaning and preprocessing (handling missing values, anomalies, and duplicates).
2. Engineer robust features and detect outliers using statistical methods (IQR).
3. Visualize correlations and distributions to uncover hidden patterns.
4. Maintain a production-quality, open-source repository suitable for data science and analytics portfolios.

## 🛠 Technologies Used
* **Language:** Python
* **Data Processing:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## 📁 Project Structure
```text
solar-power-generation-analysis/
├── data/
│   ├── raw/                # Original Kaggle dataset (gitignored)
│   └── processed/          # Cleaned dataset (solar_power_cleaned.csv)
├── notebooks/
│   └── 01_exploratory_data_analysis.ipynb
├── docs/                   # Detailed documentation and methodologies
├── LICENSE
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
└── README.md
```

## 🚀 Installation Guide

1. **Clone the repository:**
   ```bash
   git clone https://github.com/SyedMuhammadMujtabaKhalid/solar-power-generation-analysis.git
   cd solar-power-generation-analysis
   ```

2. **Set up a virtual environment (Optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. **Run Jupyter Notebook:**
   ```bash
   jupyter notebook notebooks/01_exploratory_data_analysis.ipynb
   ```

## 🧹 Data Cleaning Pipeline
Our automated data cleaning pipeline performs:
1. **Missing Value Removal:** Dropping incomplete entries to maintain data integrity.
2. **Deduplication:** Removing redundant rows.
3. **Anomaly Correction:** Filtering out negative values in `generated_power_kw`.
4. **Outlier Detection:** Utilizing the Interquartile Range (IQR) method to remove statistically significant anomalies.
5. **Feature Selection:** Subsetting the dataset to exclusively relevant environmental and target features.

*(For a visual representation of this pipeline, see [Methodology Docs](docs/methodology.md))*

## 📈 Exploratory Data Analysis & Visualizations
Extensive visual analysis was conducted using Seaborn and Matplotlib:
* **Average Power by Cloud Cover:** Categorized cloud cover into Low, Medium, and High to measure average power dropoff.
* **Radiation vs. Power Trend:** Sorting and plotting solar radiation against generated power to reveal a strong positive correlation.
* **Temperature Boxplots:** Visualizing the spread and variance of power generation across different temperature ranges.
* **Scatter Distributions:** Highlighting clustering and density in the relationship between radiation and generated power.

## 💡 Key Insights & Results
1. **Radiation Dependency:** As expected, solar radiation is the primary driver of power generation, showing a strong positive, nearly linear trend.
2. **Temperature Impact:** Extreme temperatures show a notable impact on power generation variance, highlighting the thermal sensitivity of solar panels.
3. **Cloud Cover Effect:** High cloud cover significantly diminishes average generated power, validating the categorization applied during feature engineering.

## 🔮 Future Improvements
* **Machine Learning:** Implement predictive models (e.g., Random Forest, XGBoost) to forecast power generation based on weather data.
* **Time Series Analysis:** Incorporate timestamp data to analyze seasonality, daily peaks, and cyclic behavior.
* **Dashboard Integration:** Build an interactive Streamlit or Dash web app for real-time data exploration.

## 📜 License & References
* This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.
* Data provided by [stucom on Kaggle](https://www.kaggle.com/datasets/stucom/solar-energy-power-generation-dataset).

---
<div align="center">
  <i>Developed and Maintained by Syed Muhammad Mujtaba Khalid</i>
</div>
