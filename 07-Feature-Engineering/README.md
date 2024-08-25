This folder contains scripts and documentation related to feature engineering processes. 

# Feature Engineering for Electric Vehicle (EV) Analysis

## Overview
This project involves the analysis of electric vehicle (EV) adoption across various counties and cities in Washington State. To effectively achieve our business objectives, we performed feature engineering to create new features that enhance our dataset. These features are crucial for understanding geographic distribution, market penetration, growth trends, and consumer behavior related to EV adoption.

## Business Objectives

1. **Geographic Distribution Analysis**
   - **Objective:** Identify counties and cities in Washington State with the highest and lowest numbers of electric vehicles (EVs).
   - **Goal:** Understand regional adoption trends and pinpoint areas that may benefit from additional support or incentives to boost EV adoption.

2. **Market Penetration and Growth Trends**
   - **Objective:** Analyze the change in the number of electric vehicles over time across different regions.
   - **Goal:** Understand the growth trends of EV adoption and project future adoption rates to aid stakeholders in planning.

3. **Consumer Behavior Analysis**
   - **Objective:** Examine the preferences for different types of EVs (Battery Electric Vehicles vs. Plug-in Hybrid Electric Vehicles) across regions.
   - **Goal:** Provide insights to car manufacturers and policymakers on regional preferences, helping them tailor offerings and incentives accordingly.

## Feature Engineering

### 1. Vehicle Age
   - **What I Did:** Created the `Vehicle Age` feature by subtracting the `Model Year` from the current year.
   - **Purpose:** To understand how the age of vehicles impacts EV adoption trends. This feature can highlight trends such as early adopters versus recent purchasers.
   - **Business Objective Addressed:** 
     - **Market Penetration and Growth Trends**: Helps analyze the correlation between vehicle age and the market penetration of EVs over time.

### 2. Manufacturer Proportion by Region
   - **What I Did:** Added the `Make_Proportion` feature, which calculates the proportion of vehicles from each manufacturer within each county.
   - **Purpose:** To capture the dominance of specific manufacturers within regions, which could influence overall EV adoption rates.
   - **Business Objective Addressed:** 
     - **Geographic Distribution Analysis**: Identifies regions where certain manufacturers are more prevalent, potentially due to regional preferences or marketing efforts.

### 3. CAFV Eligibility Category
   - **What I Did:** Simplified the `Clean Alternative Fuel Vehicle (CAFV) Eligibility` into a binary feature named `CAFV Eligibility Category`.
   - **Purpose:** To make it easier to analyze the impact of CAFV eligibility on EV adoption, particularly in terms of incentives.
   - **Business Objective Addressed:** 
     - **Consumer Behavior Analysis**: Assists in understanding how CAFV eligibility influences consumer choices between BEVs and PHEVs.

### 4. Electric Vehicle Type Encoding (BEV vs. PHEV)
   - **What I Did:** Encoded the `Electric Vehicle Type` (BEV vs. PHEV) into a numerical format as `EV_Type_Encoded`.
   - **Purpose:** To facilitate the use of this categorical data in machine learning models that require numerical inputs.
   - **Business Objective Addressed:** 
     - **Consumer Behavior Analysis**: Enables analysis of regional preferences for BEVs versus PHEVs.

### 5. Urban and CAFV Eligibility Interaction
   - **What I Did:** Created the `Urban_CAFV_Interaction` feature by combining the `Urban` and `CAFV Eligibility` columns.
   - **Purpose:** To capture the combined effect of urbanization and CAFV eligibility on EV adoption, which might reveal how these factors interact in influencing regional adoption patterns.
   - **Business Objective Addressed:** 
     - **Geographic Distribution Analysis**: Helps identify areas where the interaction of urbanization and CAFV eligibility impacts EV adoption rates.

### 6. Yearly Growth Rate
   - **What I Did:** Calculated the `Yearly_Growth_Rate` feature by grouping data by `County` and `Model Year`, then computing the percentage change in the number of EVs year-over-year.
   - **Purpose:** To track the year-over-year growth in EV adoption within each county, helping identify regions with accelerating or declining growth.
   - **Business Objective Addressed:** 
     - **Market Penetration and Growth Trends**: Provides insights into how EV adoption is growing or slowing down across different regions.

## Conclusion
The feature engineering process was meticulously designed to create features that directly support the analysis required to meet our business objectives. Each feature was developed to capture essential aspects of the data, ensuring that the subsequent modeling and analysis phases are both relevant and insightful.

