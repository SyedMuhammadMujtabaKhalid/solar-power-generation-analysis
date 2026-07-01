# Solar Energy Power Generation Analysis

## Project Overview
This project focuses on analyzing the impact of various weather and environmental factors on solar power generation. By conducting Exploratory Data Analysis (EDA) on telemetry data, we aim to uncover how dynamic conditions like solar radiation, ambient temperature, and cloud cover influence the overall efficiency and power output of solar energy systems. 

## Key Research Questions
The analysis addresses the following fundamental questions:
* How strongly does solar radiation correlate with the amount of power generated?
* What is the statistical impact of ambient temperature on the efficiency of solar panels?
* How does varying cloud cover diminish the average solar power generation?
* Can we identify underlying anomalies or outliers in the power generation data?

## Tech Stack
This project was built using the following tools and libraries:
* **Python**: The core programming language used for analysis.
* **Pandas**: For robust data manipulation, cleaning, and preprocessing.
* **Matplotlib**: For foundational data visualization and trend plotting.
* **Seaborn**: For advanced, statistically appealing visual distributions.

## How to Run

Follow these instructions to run the analysis locally:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/SyedMuhammadMujtabaKhalid/solar-power-generation-analysis.git
   cd solar-power-generation-analysis
   ```

2. **Install Dependencies:**
   Ensure you have Python installed, then install the required libraries via pip:
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

3. **Run the Jupyter Notebook:**
   Launch Jupyter Notebook to view the code and visualizations:
   ```bash
   jupyter notebook notebooks/01_exploratory_data_analysis.ipynb
   ```

## 💡 Key Insights

Based on the data analysis, we discovered the following key insights:
* **Solar Radiation Dominance:** Solar radiation is the most significant driving factor. There is a strong, nearly linear positive correlation between the amount of shortwave solar radiation received and the power generated.
* **Temperature Sensitivity:** While higher solar radiation naturally increases ambient temperature, extreme temperatures can slightly alter panel efficiency, as shown by the varied power generation distribution at differing temperature ranges. 
* **Cloud Cover Attrition:** As expected, significant cloud cover directly impedes power generation. The data confirms a sharp decline in average power output on days categorized with high cloud cover compared to clear, low-cover days.
