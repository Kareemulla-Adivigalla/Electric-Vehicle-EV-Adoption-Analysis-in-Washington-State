# Electric Vehicle (EV) Adoption in Washington State: Modeling and Analysis

## Overview
This project aims to analyze the adoption of electric vehicles (EVs) across various counties and cities in Washington State. The goal is to understand geographic distribution, market penetration, and consumer preferences to inform policy decisions, marketing strategies, and support programs for EV adoption.

## Objectives and Business Goals

### 1. Geographic Distribution Analysis
- **Objective:** Identify regions with the highest and lowest numbers of EVs.
- **Goal:** Understand regional adoption trends and suggest areas for additional support or incentives.

### 2. Market Penetration and Growth Trends
- **Objective:** Analyze the growth of EV adoption over time and project future adoption rates.
- **Goal:** Help stakeholders plan infrastructure and marketing strategies accordingly.


## Data Preparation and Feature Engineering

### Initial Data Setup
- **Data Source:** EV registration data from Washington State.
- **Data Cleaning:** Missing values were handled by imputing medians or dropping columns/rows as needed.

### Feature Engineering
- **Created Features:**
  - `Vehicle Age`: Calculated as the difference between the current year and the `Model Year`.
  - `Make_Proportion`: The proportion of EVs made by a particular manufacturer in a given region.
  - `Urban_CAFV_Interaction`: Interaction term between urban status and CAFV eligibility to understand the combined effect on EV adoption.
  - `Yearly_Growth_Rate`: The annual growth rate of EV adoption within each county.

- **Purpose:** These features were created to capture relevant information for modeling geographic distribution, growth trends, and consumer preferences.

## Handling Missing Values
- **Initial Check:** Identified missing values in the `Make_Proportion` column.
- **Solution:** Columns with missing values were dropped to ensure model accuracy and reliability.

## Modeling and Analysis

### 1. Geographic Distribution Analysis
- **Model:** Logistic Regression
- **Target:** Binary classification of regions into high or low EV adoption.
- **Features Used:** `Make_Proportion`, `Urban`, `CAFV Eligibility`, `Dominant_Manufacturer_Proportion`, `Vehicle Age`, `Yearly_Growth_Rate`
- **Outcome:** Identified key factors driving high and low adoption areas, with accuracy metrics validating the model's reliability.

### 2. Market Penetration and Growth Trends
- **Model:** Time Series Forecasting (ARIMA)
- **Objective:** Forecast future EV adoption based on historical trends.
- **Outcome:** Forecasting provided insights into future adoption trends, indicating potential growth areas.


## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** `pandas`, `sklearn`, `matplotlib`, `seaborn`, `imbalanced-learn`, `statsmodels`
- **Data Visualization:** Matplotlib, Seaborn
- **Modeling:** Logistic Regression, ARIMA

## Recommendations and Next Steps
- **Infrastructure Investment:** Focus on regions with low adoption rates to enhance EV infrastructure.
- **Targeted Incentives:** Introduce incentives in regions identified as potential growth areas.
- **Further Analysis:** Expand the analysis to include economic and demographic data for a more comprehensive understanding of EV adoption.

## How to Run This Analysis
1. Clone this repository to your local machine.
2. Ensure all necessary libraries are installed via `pip install -r requirements.txt`.
3. Run the provided Jupyter Notebooks to reproduce the analysis and visualizations.

## Conclusion
This project successfully identified key trends in EV adoption across Washington State and provided actionable recommendations to stakeholders. The analysis highlights the importance of targeted infrastructure investments and incentives to promote EV adoption in underrepresented regions.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
