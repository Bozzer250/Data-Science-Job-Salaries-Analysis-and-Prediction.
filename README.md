# Data Science Job Salaries Analysis and Prediction.
According to the 2020 LinkedIn U.S. Emerging Jobs Report, data science has experienced continued growth on a tremendous scale in recent years. Across nearly every industry, organizations are competing for data science professionals to leverage their data and drive smart business decisions. However, since the supply of data professionals has not yet caught up with the demand, the competition between companies in hiring these professionals is fierce compared to in other tech sectors. As a result, employers are willing to pay top salaries to talented data scientists.

Notwithstanding the profitable honeymoon this field is experiencing, it is important to note that the data science salaries can range considerably across professionals. Employers take into account several factors when deciding how much to pay, including experience, skills, job title, or company size.

# LinkedIn Profile
For any queries regarding about this project contact me.

- Link [Click here](https://www.linkedin.com/in/naloys/)

# Acquisition of data
The Data Science salary data (Salary_Data.csv) that we will use for the analysis is obtained from Kaggle.

- Link [Download here](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries?resource=download)

# Data set
<img width="1247" alt="dataset" src="https://github.com/Bozzer250/Data-Science-Job-Salaries-Analysis-and-Predict/assets/122544599/90a420f8-bc40-4555-86e2-ea866ff72ca0">

## Observation:

• The dataset consists of 12 columns and 607 rows.

- Unnamed: 0
- work_year
- experience_level
- employment_type
- job_title
- salary
- salary_currency
- salaryinusd
- employee_residence
- remote_ratio
- company_location
- company_size

- Column `Unnamed`: 0 needs to be removed, as it is unecessary columns.

- The names of each column are lowercase.

- The values of the `experience_level`, `employment_type`, `remote_ratio`, and `company_size` columns need to be redefined.

- `work_year`, `salary`, `salary_in_usd`, and `remote_ratio` columns are numeric.

# Data Cleansing
- Removed unwanted columns: 'Unnamed: 0'.

- Dataframe has no missing values.

- Drop 42 duplicate rows found.

- Renaming the column value

  - experience_level : EN = Entry-level, MI = Mid-level, SE = Senior-level, EX = Expert-level
  - employment_type : PT = Part-time, CT = Contract, FT = Full-time, FL = Freelance
  - remote_ratio.replace : 0 = Onsite, 50 = Hybrid, 100 = Remote
  - company_size.replace : S = Small, M = Medium, L = Large
    
- After renaming the column value, the dtype of the remote_ratio column changes to object.

## Exploratory Data Analysis (EDA)

### Creating boxplot to see outliers in data.
