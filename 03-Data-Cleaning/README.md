This folder contains scripts and documentation for cleaning and preprocessing the data. 


 Data Cleaning Process
---

 1. Data Loading
* I began by loading the raw dataset containing information on electric vehicles registered in Washington state. The dataset was loaded into a pandas DataFrame for further processing.

 2. Initial Data Exploration
I conducted an initial exploration of the dataset to understand its structure, data types, and identify any immediate data quality issues. This included:
* Checking the first few rows of the dataset.
* Summarizing the dataset with `.info()` and `.describe()` methods to get an overview of the data types, non-null counts, and basic statistics.

 3. Handling Missing Values
I identified missing values in several columns:
* **County, City, Postal Code, Electric Utility, and 2020 Census Tract:** I chose to drop rows with missing values in these columns since the number of missing entries was minimal.

* **Legislative District:** I chose to drop the column, because of it's not critical for this analysis.

* **Vehicle Location:** Since only a few values were missing, I dropped rows where this column was missing.


 4. Correcting Data Types
* I ensured that all columns had the correct data types:
* Converted `Postal Code` to a string since it represents categorical geographic data.
* Ensured `Model Year` was an integer.


 5. Handling Outliers
* I identified potential outliers in the numerical columns `Electric Range` and `Base MSRP`:
* Used boxplots to visualize these outliers.
* Capped the outliers at the 1st and 99th percentiles to reduce their impact on the analysis.


 6. Removing Duplicates
* I checked for and removed any duplicate rows to ensure the dataset's integrity.


 7. Final Data Quality Check
* A final check was conducted to ensure all data cleaning steps were successful:
* Verified that there were no remaining missing values.
* Confirmed that data types were appropriate and consistent.
* Reviewed the cleaned dataset to ensure accuracy.


 8. Saving the Cleaned Dataset
Finally, I saved the cleaned dataset to a new CSV file for future analysis.



