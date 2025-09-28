# Kaggle Data Science Survey 2021 - Data Cleaning and Insight Generation
## Project Overview
This project involves working with the **Kaggle Data Science Survey 2021** dataset to perform data cleaning, preprocessing, and generate meaningful insights from survey respondents’ answers. The survey contains real-world data with missing values, duplicates, and inconsistent formatting that requires cleaning before analysis.
The main goals of this project are:
- Clean the dataset to handle missing and duplicate data
- Apply label encoding to categorical variables
- Extract top insights about respondents' behavior and preferences
- Visualize the insights in a dashboard
- Save cleaned data and dashboard outputs as files for further use
## Dataset
- **Dataset Name:** Kaggle Data Science Survey 2021  
- **Source:** [Kaggle Datasets](https://www.kaggle.com/kaggle/kaggle-survey-2021)  
- **File Used:** `kaggle_survey_2021_responses.csv`  
- **Description:** The dataset contains responses from thousands of data science practitioners globally, including demographic information, role, tools, programming languages, and machine learning platforms used.
- 
## Environment and Libraries

- Python 3.x  
- pandas  
- matplotlib  
- seaborn  
- scikit-learn (for Label Encoding)

## Code Overview
### 1. Data Loading
- The survey data is loaded from a CSV file.
- To avoid dtype warnings due to mixed data types, `low_memory=False` is used during loading.
### 2. Data Cleaning
- The first row is removed if it contains duplicate headers.
- Columns with more than 50% missing values are dropped.
- Duplicate rows are removed.
- Missing values in key columns (like job role) are handled by filtering out nulls.
### 3. Feature Engineering
- Label encoding is applied to the job role column (`Q5`) to convert categorical values into numeric labels.
### 4. Insight Generation
- Top 5 countries by respondents.
- Top 5 job roles.
- Top 5 programming languages used.
- Top 5 education levels.
- Top 5 machine learning platforms used.
### 5. Visualization
- A multi-panel dashboard is created using matplotlib and seaborn.
- Bar charts display each insight clearly.
- The dashboard image is saved to a PNG file.
### 6. Output Saving
- Cleaned dataset is saved as `cleaned_kaggle_survey_2021.csv`.
- Dashboard image saved as `kaggle_survey_2021_insights_dashboard.png`.
