# Electric Vehicle (EV) Adoption: Exploratory Data Analysis (EDA)

## Overview
This project presents an in-depth Exploratory Data Analysis (EDA) focused on understanding the adoption of electric vehicles (EVs) across various regions. The aim was to explore patterns, trends, and factors influencing EV adoption, specifically differentiating between Battery Electric Vehicles (BEVs) and Plug-in Hybrid Electric Vehicles (PHEVs).

## Objectives
- **Analyze the distribution of EVs:** Assess how EVs are distributed across counties and cities.
- **Compare BEVs and PHEVs adoption:** Understand the preference trends between BEVs and PHEVs.
- **Examine correlation factors:** Identify key factors such as geographic location, EV range, and incentives that correlate with higher adoption rates.
- **Provide actionable insights:** Offer recommendations for boosting EV adoption based on analysis.

## Approach

### 1. Data Collection and Preparation
- **Data Source:** The dataset was gathered from publicly available EV registration data.
- **Data Cleaning:** The dataset was cleaned to handle missing values, correct inconsistencies, and ensure accuracy in county and city names.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** pandas, matplotlib, seaborn
- **Data Visualization:** Matplotlib, Seaborn
- **IDE:** Jupyter Notebook
- **Version Control:** Git

### 2. Exploratory Data Analysis (EDA)
- **Descriptive Statistics:** Basic statistics were calculated to understand the central tendencies and dispersion of the data.
- **Visualization:** Various visual tools were used to analyze the distribution of EVs across different regions and vehicle types.
  - **Tools Used:** Python's `matplotlib` and `seaborn` libraries were extensively utilized for creating bar charts, line graphs, heatmaps, and box plots.
- **Segmentation Analysis:** Data was segmented by counties and cities to compare EV concentrations, focusing on the top 20 regions.
- **Trend Analysis:** Year-over-year trends in EV adoption were analyzed to understand the growth patterns.

### 3. Key Insights and Findings
- **BEV Dominance:** BEVs significantly outnumber PHEVs, with over 160,000 BEVs compared to 60,000 PHEVs, showing a strong consumer preference for fully electric vehicles.
- **Geographic Disparities:** King County leads in EV adoption with over 100,000 registered vehicles, making it a major hub, while rural counties show very low adoption rates.
- **Popular Makes and Models:** Tesla dominates the market, with the Model Y and Model 3 being the most popular EV models.
- **Electric Range and MSRP:** Higher MSRP vehicles tend to have greater electric ranges, particularly those eligible for Clean Alternative Fuel Vehicle (CAFV) status.

### 4. Recommendations
- **Infrastructure Investment:** Increase EV charging stations, particularly in rural areas and cities with lower adoption rates such as Pierce and Yakima counties.
- **Targeted Incentives:** Introduce incentives tailored to lower-income regions and areas with low adoption to encourage EV purchases.
- **Benchmarking Success:** Use successful regions like King County and Seattle as models to replicate in other areas, focusing on infrastructure and incentives.

### 5. Conclusion
- **Final Insights:** The analysis revealed significant trends and provided actionable recommendations to enhance EV adoption. The results emphasize the importance of continued infrastructure development and targeted incentives.

## How to Run This Analysis
1. Clone this repository to your local machine.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Open the Jupyter Notebook `Exploratory_Data_Analysis_on_County,_city,_Model_Year_and_Electric_Vehicle_Type.ipynb`.
4. Execute the cells sequentially to reproduce the analysis and visualizations.
5. Review the final insights and recommendations in the notebook’s conclusion section.

## Acknowledgments
- Data was sourced from publicly available datasets on EV registrations in Washington State.
- Visualization techniques were inspired by industry-standard data analysis practices.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
