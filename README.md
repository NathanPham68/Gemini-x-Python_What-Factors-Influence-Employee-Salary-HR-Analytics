# [Gemini x Python] What Factors Influence Employee Salary? — HR Analytics

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/2862788b-ba86-4d1f-b3a2-e58c3d613220" />

## I. Introduction

This project explores the key factors that impact employee salaries using a structured HR dataset. The dataset contains over 6,700 records with demographic and professional attributes, including Age, Gender, Education Level, Job Title, Years of Experience and Salary.

Through data cleaning, descriptive statistics and visual analytics, the project aims to uncover insights such as:

* How experience and education influence salary levels

* Gender-based salary disparities

* Salary variations across different job titles and industries

The project leverages Python (Pandas, Matplotlib, Seaborn) for data processing and exploratory analysis and Power BI for interactive data visualization and reporting.

## Part I: Import Data

[**Link to code**](https://colab.research.google.com/drive/1ebKqIqizgeXuSTMzkZ8TbTQPa2B2BkO0?usp=sharing)

```ruby
Generate Google Colab code in separate cells to import a CSV file, perform data overview.
Dataset: Salary data, columns:
- Age
- Gender
- Education level
- Job Title
- Years of Experience
- Salary
Goal: analyse salary trends

Here's a breakdown of the cells I'd like:
**CELL 1: SETUP & IMPORT**
- Import all necessary libraries (pandas, numpy, matplotlib, seaborn, plotly)
- Use Google Colab file upload widget to import a CSV file from my local machine.
- Load the data into a pandas DataFrame.
- Define the following columns:
+ Categorical columns: ['Gender','Education Level','Job Title']
+ Numerical columns: ['Age','Years of Experience','Salary']
- Convert categorical columns to 'category' dtype.
- Attempt to convert numerical columns to a suitable numerical type, handling errors.
- Print the identified categorical and numerical columns.
- Display the DataFrame's info().

**CELL 2: DATA OVERVIEW**
- Print the shape of the DataFrame.
- Print information about the DataFrame using info().
- Print descriptive statistics of the DataFrame using describe().
- Print the data types of each column using dtypes.
- Display the first 5 rows of the DataFrame using display(df.head()).
- Print the column names as a list.
- Print the number of missing values per column.
Make sure to add markdown cells before each code cell to explain the purpose of the code block.
```

### Setup and data loading

<img width="1300" height="673" alt="image" src="https://github.com/user-attachments/assets/9cce865a-0ff0-44a8-b721-fefb23bb7ab3" />

### Data overview

<img width="1300" height="698" alt="image" src="https://github.com/user-attachments/assets/bb8a5f55-cf76-4732-b0bf-aaf9b77078c7" />

### Analyze salary trends

<img width="1300" height="597" alt="image" src="https://github.com/user-attachments/assets/2f47a51a-4b05-4de3-9f76-a8d7513d3165" />

<img width="1300" height="647" alt="image" src="https://github.com/user-attachments/assets/14e0451c-79bb-4392-80c8-8dede8178299" />

### Summary

#### Data Analysis Key Findings

*   The dataset contains 6704 rows and 6 columns: 'Age', 'Gender', 'Education Level', 'Job Title', 'Years of Experience', and 'Salary'.
*   There are no missing values in any of the columns.
*   Numerical columns ('Age', 'Years of Experience', 'Salary') have strong positive correlations with each other, indicating that as age and years of experience increase, salary also tends to increase.
*   The average salary varies significantly across different 'Education Level' and 'Job Title' categories.

#### Insights or Next Steps

*   Further investigation into specific job titles within each education level could provide more granular insights into salary variations.
*   Analyzing the impact of 'Gender' on salary, while controlling for other factors, could be a valuable next step to identify potential gender pay gaps.

## Part II: EDA

[**Link to code**](https://colab.research.google.com/drive/1ebKqIqizgeXuSTMzkZ8TbTQPa2B2BkO0?usp=sharing)

```ruby
Based on my setup dataset from Step 1, assess data quality, investigate outlier if any, treat outlier, missing value and normalize data. Generate comprehensive data cleaning workflow:
**CELL 1: DATA QUALITY ASSESSMENT & OUTLIER DETECTION**
- Detect outliers using IQR, Z-score methods 
- Visualize outliers with boxplots and scatter plots 
- Detect duplicates and inconsistent formats 
- Missing data patterns analysis 
- Generate comprehensive data quality report 

**CELL 2: OUTLIER INVESTIGATION** 
- Show outlier records for business review 
- Statistical significance of outliers 
- Pattern analysis of extreme values 
- Document outliers for cleaning decisions

**CELL 3: OUTLIER TREATMENT DECISIONS** 
- Provide multiple options for each outlier: remove, keep, transform, cap 
- Business-logic based outlier handling 
- Document all outlier treatment decisions

**CELL 4: MISSING DATA HANDLING** 
- Automated missing value treatment based on column type 
- Imputation strategies for numerical columns 
- Mode/most frequent for categorical columns 
- Document all cleaning decisions 

**CELL 5: DATA TYPE OPTIMIZATION & STANDARDIZATION** 
- Convert columns to appropriate data types automatically 
- Parse dates if detected 
- Remove duplicates 
- Standardize text formatting (trim spaces, case consistency) 
- Normalize/standardize numerical columns if needed 

**CELL 6: CLEANED DATA VALIDATION** 
- Before vs after comparison 
- Validation of cleaning results (including outlier treatment) 
- Final data quality report 
- Export cleaned dataset option 

Customize cleaning approach based on my specific data issues and outlier findings from Step 1.
```

### Data quality assessment & outlier detection

<img width="1300" height="716" alt="image" src="https://github.com/user-attachments/assets/746b4d3b-0e8f-41c7-9b44-026a581e01f8" />

<img width="1300" height="655" alt="image" src="https://github.com/user-attachments/assets/28de0c2d-6b88-4553-b560-1186855626a0" />

<img width="1300" height="672" alt="image" src="https://github.com/user-attachments/assets/123b8261-4362-4cfa-a25b-e7d5e64b4045" />

### Outlier investigation

<img width="1300" height="584" alt="image" src="https://github.com/user-attachments/assets/5eed119d-968c-4bbe-8246-a445e6e99e98" />

### Outlier treatment decisions

<img width="1300" height="606" alt="image" src="https://github.com/user-attachments/assets/79fbbb99-73f2-4957-b966-ea74aba38184" />

### Missing data handling

<img width="1300" height="607" alt="image" src="https://github.com/user-attachments/assets/b20096e6-208e-4744-8b30-9c58ce126033" />

### Data type optimization & standardization

<img width="1300" height="608" alt="image" src="https://github.com/user-attachments/assets/1fdb5448-b87c-4fbb-abad-d10c177b0a17" />

### Cleaned data validation

<img width="1300" height="664" alt="image" src="https://github.com/user-attachments/assets/bc10d1e2-6686-41cf-a369-59d9706bee47" />

### Summary

#### Data Analysis Key Findings

*   Outlier detection using the IQR method identified 123 outliers in 'Age' and 75 in 'Years of Experience'. The Z-score method (threshold 3) detected no outliers.
*   The initial dataset contained 4912 duplicate rows, which were subsequently removed, reducing the dataset size from 6704 to 1792 rows.
*   Categorical columns like 'Education Level' had inconsistent formatting (e.g., "Bachelor's Degree", "Bachelor's", "PhD", "phD"), which was standardized to lowercase and stripped whitespace.
*   Missing values were found in 'Education Level' (1), 'Salary' (2), 'Age' (1), and 'Years of Experience' (2) in the final cleaned dataset, despite the imputation steps. Categorical columns also showed 'nan' as a unique value after cleaning.
*   Outliers in 'Age' and 'Years of Experience' were primarily associated with older, highly experienced individuals with higher salaries, often holding PhDs and in roles like "Software Engineer Manager."
*   Numerical columns ('Age', 'Years of Experience', 'Salary') have significantly different scales, indicating a need for scaling if the data is to be used for certain machine learning algorithms.

#### Insights or Next Steps

*   Investigate the remaining missing values in the cleaned dataset to understand why they persist after imputation and refine the missing data handling process if necessary.
*   Address the 'nan' unique values in categorical columns, potentially by treating them as a distinct category or re-evaluating the categorical imputation strategy.

## Part III: Analysis

[**Link to code**](https://colab.research.google.com/drive/1ebKqIqizgeXuSTMzkZ8TbTQPa2B2BkO0?usp=sharing)

```ruby
Based on my cleaned and outlier-treated dataset from Step 2, create comprehensive EDA code for Google Colab. 
Generate systematic EDA code: 
**UNIVARIATE ANALYSIS** 
- Distribution analysis for all cleaned numerical columns 
- Frequency analysis for all categorical columns 
- Summary statistics on cleaned data 

**BIVARIATE ANALYSIS** 
- Correlation analysis between all variables 
- Relationship exploration based on cleaned data 
- Cross-variable comparisons without outlier noise 

**MULTIVARIATE ANALYSIS** 
- Pattern discovery across multiple variables 
- Advanced visualizations on clean data 
- Segmentation insights 

**BUSINESS INSIGHTS** 
- Key findings summary from cleaned data 
- Impact of outlier treatment on insights 
- Recommendations based on discovered patterns 
- Next steps for deeper analysis Work with my cleaned, outlier-treated dataset for accurate and reliable analysis results.
```

### Univariate analysis

<img width="1300" height="645" alt="image" src="https://github.com/user-attachments/assets/baae10d2-dc7e-423e-b720-89c2f8f9f301" />

<img width="1300" height="652" alt="image" src="https://github.com/user-attachments/assets/b417fcff-30f6-4c0a-b65f-9bdd93a72b86" />

### Bivariate analysis

<img width="1300" height="685" alt="image" src="https://github.com/user-attachments/assets/613c230e-80af-4604-97a0-02d915ebb265" />

<img width="1300" height="707" alt="image" src="https://github.com/user-attachments/assets/d3190202-eff6-4071-b36a-3cf3c6cc9249" />

### Multivariate analysis

<img width="1300" height="671" alt="image" src="https://github.com/user-attachments/assets/e1ee2516-beb0-4511-b121-1f4c32c35403" />

<img width="1300" height="674" alt="image" src="https://github.com/user-attachments/assets/f0786f9f-85fd-4f9c-a18e-ac053b23f2e1" />

### Business insights

<img width="1300" height="592" alt="image" src="https://github.com/user-attachments/assets/e6ed3c02-70e5-4869-848c-f3caa0ecec24" />

### Summary

#### Data Analysis Key Findings

*   **Salary Distribution:** The salary distribution is right-skewed, with a long tail towards higher salaries.
*   **Numerical Variable Relationships:** Age, Years of Experience, and Salary show strong positive correlations with each other.
*   **Education Level Impact:** Higher education levels (Master's and PhD) are associated with substantially higher average salaries compared to Bachelor's degrees or High School diplomas.
*   **Gender and Salary:** A notable salary gap exists between genders, with males consistently having higher average salaries across different education levels.
*   **Job Title Diversity:** The dataset contains a wide variety of Job Titles, with certain roles in management and specialized technical fields showing higher average salaries.
*   **Impact of Cleaning:** Removing a large number of duplicate rows significantly reduced the dataset size from 6704 to 1792, leading to a more representative dataset.
*   **Cleaning Order Issues:** The order of outlier removal and duplicate removal steps in the cleaning process could be improved, as some potential outliers remained in the final dataset.
*   **Missing Values:** While imputation was performed, some missing values and 'nan' categories still remained in the final cleaned dataset, indicating potential areas for refining the imputation process.

#### Insights or Next Steps

*   Investigate the observed gender pay gap in more detail, potentially by analyzing specific job titles or departments to pinpoint where disparities are most significant.
*   Refine the data cleaning pipeline, specifically the order of operations for duplicate removal, outlier handling, and missing value imputation, to ensure consistent and effective data quality improvement.


