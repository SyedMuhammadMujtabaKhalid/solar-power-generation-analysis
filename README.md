# Solar Energy Power Generation Analysis
**Data Visualization Pitch - Student Individual Assignment**

**Author:** Muhammad Mujtaba Khalid, Syed   
**Email:** m.syed17@campus.unimib.it  

---

## Project Overview
This project focuses on understanding the impact of weather and environmental factors, particularly solar radiation and temperature, on solar power output. By conducting Exploratory Data Analysis (EDA) on telemetry data, we aim to uncover how these dynamic conditions influence the overall efficiency and power generation of solar energy systems. 

## Key Research Questions
The analysis addresses the following fundamental questions:
* Is there a measurable relationship between solar radiation levels and electricity output?
* How does temperature variability affect the distribution and stability of power generation?
* Are there observable patterns or outliers that indicate inefficiencies or extreme operating conditions?

## Tech Stack
This project was built using the following tools and libraries:
* **Python**: The core programming language used for analysis.
* **Pandas**: For data manipulation, handling missing values, and eliminating duplicates.
* **NumPy**: For numerical operations.
* **Matplotlib & Seaborn**: For comparative, trend-based visual inspection, and anomaly detection.

## About the Data
* **Source:** Kaggle (Solar energy power generation dataset)
* **Data Characteristics:** Structured tabular data (CSV format) consisting of continuous numerical variables suitable for exploratory and descriptive analysis.
* **Limitations:**
  * Measurements may be affected by sensor calibration errors.
  * Data represents a specific geographic location, limiting generalizability.
  * Weather conditions such as dust or shading are not explicitly captured.

## How to Run

Follow these instructions to run the analysis locally:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/SyedMuhammadMujtabaKhalid/solar-power-generation-analysis.git
   cd solar-power-generation-analysis
   ```

2. **Install Dependencies:**
   Ensure you have Python installed, then install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Run the Jupyter Notebook:**
   Launch Jupyter Notebook to view the code and visualizations:
   ```bash
   jupyter notebook notebooks/01_exploratory_data_analysis.ipynb
   ```

## 💡 Key Insights

Based on the visual data analysis, we discovered the following key insights:
* **Solar Radiation Dominance:** Solar radiation exhibits a strong positive relationship with electricity generation, confirming it as the primary driver of solar energy production. Higher radiation levels consistently result in increased electricity output.
* **Temperature Sensitivity:** Power generation shows noticeable variability across temperature levels. Extreme temperatures are associated with increased dispersion and outliers. Temperature affects the stability and variability of the power generation rather than determining maximum output levels.
* **System Optimization:** The presence of outliers in power output suggests performance fluctuations under extreme environmental conditions. These trends can support energy forecasting and system optimization in renewable energy planning.

## License
A Data Visualization Study of Solar energy power generation © 2026 by Muhammad Mujtaba khalid, Syed is licensed under **CC BY-NC-SA 4.0** (Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International).
See the `LICENSE` file for more details.
