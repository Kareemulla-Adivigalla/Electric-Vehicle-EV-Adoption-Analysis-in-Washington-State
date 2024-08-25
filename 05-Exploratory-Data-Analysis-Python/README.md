This folder contains notebooks, scripts, and figures for exploratory data analysis. 


# Electric Vehicle (EV) Adoption in Washington State: Exploratory Data Analysis (EDA)

## Overview
This project focuses on the exploratory data analysis (EDA) of electric vehicle (EV) adoption across various counties and cities in Washington State. The goal was to uncover patterns, trends, and key insights into how electric vehicles are distributed, adopted, and how different factors influence this adoption.

## Objectives
- Analyze the distribution of electric vehicles across counties and cities in Washington State.
- Identify trends in the adoption of Battery Electric Vehicles (BEVs) vs. Plug-in Hybrid Electric Vehicles (PHEVs).
- Examine the correlation between EV adoption and various factors such as urbanization, infrastructure availability, and incentives.
- Provide actionable insights and recommendations to enhance EV adoption in Washington State.

## Approach

### 1. **Data Collection and Preparation**
   - **Data Source:** The dataset was sourced from publicly available EV registration data in Washington State.
   - **Data Cleaning:** The data was cleaned to handle missing values, remove duplicates, and ensure consistency in the naming of counties and cities.

### 2. **Exploratory Data Analysis (EDA)**
   - **Descriptive Statistics:** Initial analysis involved calculating basic statistics (mean, median, mode) to understand the central tendencies and spread of the data.
   - **Data Visualization:** Various charts were created to visualize the distribution of EVs across counties and cities. This included bar charts, pie charts, line graphs, and heatmaps.
     - **Tools Used:** Python's `matplotlib` and `seaborn` libraries were extensively used for data visualization.
   - **Segmentation Analysis:** The dataset was segmented by county and city to examine the concentration of EVs, BEVs, and PHEVs.
   - **Trend Analysis:** Time-series analysis was conducted to identify trends in EV adoption over the years.

### 3. **Key Insights and Findings**
   - **King County Dominance:** Identified that King County has the highest number of EVs by a significant margin, with over 100,000 registered vehicles.
   - **Urban vs. Rural Adoption:** High adoption rates were observed in urban areas like Seattle, Bellevue, and Redmond, while rural areas lagged behind significantly.
   - **Preference for BEVs:** Across most counties and cities, BEVs were found to be more popular than PHEVs, particularly in King County and Seattle.
   - **Correlation Analysis:** A strong positive correlation was observed between BEV and PHEV adoption across both counties and cities.

### 4. **Recommendations**
   - **Infrastructure Investment:** Recommendations were made to enhance EV charging infrastructure, especially in rural areas and cities with moderate adoption rates like Tacoma and Everett.
   - **Targeted Incentives:** Suggested introducing specific incentives in low-adoption areas to boost EV registrations.
   - **Replication of Success:** Recommended using King County and Seattle as benchmarks for successful EV adoption, with strategies to replicate this success in other regions.

### 5. **Conclusion**
   - **Final Insights:** The project successfully identified key trends and provided actionable recommendations to improve EV adoption in Washington State. The findings emphasize the importance of targeted infrastructure investment and incentives in driving EV adoption.

## Tools and Technologies
- **Programming Language:** Python
- **Libraries:** `pandas`, `matplotlib`, `seaborn`
- **Data Visualization:** Matplotlib, Seaborn
- **IDE:** Jupyter Notebook
- **Version Control:** Git

## How to Run This Analysis
1. Clone this repository to your local machine.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Open the Jupyter Notebook `exploratory_data_analysis_on_county,_city,_model_year_and_electric_vehicle_type.ipynb`.
4. Run the cells step-by-step to reproduce the analysis and visualizations.
5. The final insights and recommendations can be found in the concluding section of the notebook.

## Acknowledgments
- Data was sourced from publicly available datasets on EV registrations in Washington State.
- Visualization inspiration was drawn from various data analysis best practices.

## License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/Kareemulla-Adivigalla/Electric-Vehicle-EV-Adoption-Analysis-in-Washington-State/blob/master/LICENSE) file for details.


