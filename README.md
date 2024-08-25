# Electric Vehicle (EV) Adoption in Washington State

## Project Overview
This project focuses on analyzing the adoption of electric vehicles (EVs) across Washington State. The primary goals were to examine the geographic distribution, and market penetration related to EVs. The insights gained from this analysis are intended to guide policy decisions, marketing strategies, and support programs to enhance EV adoption in the state.

## Business Objectives and Goals

### 1. Geographic Distribution Analysis
- **Objective:** Identify which counties and cities in Washington State have the highest and lowest numbers of EVs.
- **Goal:** Understand regional adoption trends and identify areas that may benefit from additional support or incentives to encourage higher adoption of EVs.
- **Approach:**
  1. Count and compare the number of EVs across different counties and cities.
  2. Visualize the distribution using bar charts and maps.
  3. Analyze the results to suggest where additional incentives or support might be needed.

### 2. Market Penetration and Growth Trends
- **Objective:** Analyze how the number of EVs has changed over time across different counties and cities.
- **Goal:** Understand the growth trend of EV adoption and project future adoption rates to help stakeholders plan accordingly.
- **Approach:**
  1. Group the data by year (based on Model Year) and count the number of EVs for each year.
  2. Visualize the growth trend using line charts.
  3. Compare growth trends across different regions to identify areas with rapid or slow adoption.

## Data Overview

### Dataset Description
- **Source:** The dataset includes various features such as county, city, model year, EV type, CAFV eligibility, and other relevant factors.
- **Features:**
  - VIN (1-10)
  - County
  - City
  - State
  - Postal Code
  - Model Year
  - Make
  - Model
  - Electric Vehicle Type
  - Clean Alternative Fuel Vehicle (CAFV) Eligibility
  - Electric Range
  - Base MSRP
  - DOL Vehicle ID
  - Vehicle Location
  - Electric Utility
  - 2020 Census Tract

### Data Preprocessing
- **Cleaning:** Handled missing values, removed duplicates, and standardized data formats.
- **Outlier Removal:** Removed outliers in fields like Base MSRP and Electric Range to prevent skewing results.
- **Feature Engineering:** Created new features such as `Vehicle Age`, `Make_Proportion`, `Yearly_Growth_Rate`, and others to enhance the analysis and modeling phases.

## Exploratory Data Analysis (EDA)

### Geographic Distribution Analysis
- **Objective:** Identify regions with the highest and lowest EV adoption.
- **Methodology:** 
  - Used bar charts and geographic maps to visualize the distribution of EVs across counties and cities.
  - Analyzed the data to identify patterns, such as higher adoption rates in urban areas and lower rates in rural regions.
- **Key Findings:** 
  - King County has the highest adoption of EVs.
  - Urban areas like Snohomish and Pierce counties show higher adoption rates compared to rural areas.

### Market Penetration and Growth Trends
- **Objective:** Analyze how EV adoption has grown over time.
- **Methodology:** 
  - Conducted time series analysis to track EV adoption trends by year.
  - Compared the growth rates of BEVs and PHEVs.
- **Key Findings:** 
  - There is a significant increase in EV adoption starting around 2015, with BEVs growing faster than PHEVs.

## Hypothesis Testing

### Hypothesis 1: High vs. Low CAFV Eligibility Impact
- **Test:** Chi-square test to see if there is a significant difference in EV adoption between high and low CAFV eligibility counties.
- **Result:** No significant difference was found, indicating CAFV eligibility is not the only factor driving EV adoption.

### Hypothesis 2: Urban vs. Non-Urban EV Adoption
- **Test:** Chi-square test to compare BEV adoption between urban and non-urban areas.
- **Result:** Significant difference found, with higher BEV adoption in urban areas.

## Feature Engineering

### New Features Created
- **Make_Proportion:** Proportion of a specific make within each county/city.
- **Vehicle Age:** Difference between the current year and the model year.
- **Yearly_Growth_Rate:** Growth rate of EVs year-over-year.
- **Urban_CAFV_Interaction:** Interaction between Urban and CAFV eligibility to assess combined impact. etc.,
- **Purpose:** These features were created to enhance the predictive power of the models and align the data more closely with business objectives.

## Modeling and Analysis

### Geographic Distribution Analysis
- **Modeling:** Random Forest Classifier to predict high/low adoption areas based on features like `Make_Proportion`, `Urban`, `CAFV Eligibility`, etc.
- **Outcome:** Accurate prediction of high adoption areas, with King County leading.

### Market Penetration and Growth Trends
- **Modeling:** Time Series Forecasting using ARIMA and Prophet to predict future adoption rates.
- **Outcome:** Projected continued growth in BEV adoption, particularly in urban areas.

## Interpretation and Reporting

### Key Findings
- **King County Dominance:** King County leads in EV adoption, with urban areas showing significantly higher rates.
- **BEV Growth:** BEVs are becoming increasingly popular, particularly in urban regions.

### Actionable Recommendations
- **Expand Infrastructure:** Increase EV charging stations in rural areas to boost adoption.
- **Targeted Incentives:** Implement specific incentives in low-adoption regions.
- **Support BEV Growth:** Focus on BEV infrastructure and marketing efforts, especially in regions with strong adoption trends.

## Tools and Technologies

- **Python:** Data preprocessing, EDA, feature engineering, and modeling.
- **Pandas:** For data manipulation and analysis.
- **Matplotlib/Seaborn:** Visualization of data and results.
- **Power BI:** Creation of interactive dashboards.
- **Jupyter Notebook:** For conducting and documenting the analysis.
- **Scikit-learn:** Machine learning models and evaluation.
- **ARIMA/Prophet:** Time series forecasting models.

## Dashboard and Presentation

### Power BI Dashboard
- **Pages:** Executive Summary, Geographic Distribution, Market Penetration, Key Findings, and Actionable Recommendations.
- **KPIs:** Total EVs by County/City, EV Growth Rate, BEV/PHEV Distribution.
- **Visuals:** Bar charts, line graphs, maps, and pie charts.

### Presentation
- **Content:** Overview, EDA, Key Findings, Recommendations.
- **Tools:** Microsoft PowerPoint, integrating visuals from Power BI and Python.

## Conclusion
This project successfully analyzed EV adoption trends across Washington State, providing actionable insights and recommendations. The analysis and models offer a clear understanding of regional adoption patterns, and growth trends, guiding future policy and strategic decisions to enhance EV adoption.

---

This README file documents the entire project process, from data collection to analysis, modeling, and reporting, ensuring clarity and comprehensive coverage of all aspects of the work.
