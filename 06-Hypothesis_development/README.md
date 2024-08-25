This folder contains documents related to hypothesis development and testing. 

Electric Vehicle (EV) Adoption Hypothesis Testing

Overview

This project focuses on testing hypotheses related to the adoption of electric vehicles (EVs) across various regions. The objective is to understand the factors influencing EV adoption, including the impact of urbanization, CAFV eligibility, and the dominance of certain manufacturers or models in specific regions.

Hypotheses Tested

Hypothesis 1: Urbanization and BEV Adoption
Objective: To test whether there is a significant difference in the adoption of Battery Electric Vehicles (BEVs) between urban and non-urban areas.
Null Hypothesis (H0): There is no significant difference in the proportion of BEVs compared to PHEVs between urban and non-urban areas.
Alternative Hypothesis (H1): Urban areas have a significantly higher proportion of BEVs compared to PHEVs than non-urban areas.

Results:

Chi-square Statistic: 744.60
P-Value: 6.00e-164

Conclusion: 

Reject the null hypothesis. There is a significant difference in BEV adoption between urban and non-urban areas, indicating that urbanization plays a significant role in BEV adoption.


Hypothesis 2: CAFV Eligibility and EV Adoption

Objective: To test whether counties with higher CAFV (Clean Alternative Fuel Vehicle) eligibility rates have higher overall EV adoption rates.

Null Hypothesis (H0): There is no significant difference in EV adoption rates between counties with high CAFV eligibility and those with low CAFV eligibility.
Alternative Hypothesis (H1): Counties with higher CAFV eligibility rates have significantly higher EV adoption rates compared to those with lower CAFV eligibility rates.

Results:

Chi-square Statistic: 0.0
P-Value: 1.0

Conclusion: 

Fail to reject the null hypothesis. There is no significant difference in EV adoption rates between high and low CAFV eligibility counties. This suggests that CAFV eligibility does not significantly impact overall EV adoption rates.


Tools and Technologies

Programming Language: Python
Libraries Used:
pandas: For data manipulation and analysis.
scipy.stats: For performing statistical tests (Chi-square test).
matplotlib and seaborn: For data visualization.


How to Reproduce the Analysis

Load the Dataset: Ensure you have access to the cleaned dataset, final_after_outlier_cleaned_data.csv.
Prepare the Data: Follow the steps to categorize regions into urban vs. non-urban areas, classify CAFV eligibility, and focus on specific manufacturers/models for the third hypothesis.
Perform Hypothesis Testing: Use the provided Python code snippets to conduct chi-square tests and interpret the results.


Interpret Results: Compare the p-values to a significance level (e.g., 0.05) to decide whether to reject or fail to reject each null hypothesis.


Key Findings and Implications
Urbanization significantly influences BEV adoption, with urban areas showing a higher preference for BEVs compared to non-urban areas.
CAFV eligibility does not have a significant impact on overall EV adoption rates, suggesting that other factors may be more influential.

