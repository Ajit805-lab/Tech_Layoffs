# Tech Layoffs Analysis

## 🔍 Overview
    This project provides a detailed analysis of global company layoffs using a comprehensive dataset containing 
    company-wise information such as location, industry, funding stage, and layoffs over time.
## 📁 Dataset UsedSource: 
    Source: Sample Superstore Dataset(Available via Kaggle)

    Data Attributes: Company, Location_HQ, Country, Continent, Laid_Off,	Date_layoffs,	Percentage,
    
    Company_Size_before_Layoffs, Company_Size_after_layoffs, Industry, Stage, Money_Raised_in_$_mil, Year, lat, lng.

## 📷 Dataset Overview

<img width="1152" height="643" alt="Screenshot 2025-07-19 182133" src="https://github.com/user-attachments/assets/da69a274-897a-4c0f-80f4-471c4e553322" />

## 🎯 Objectives
    Analyze the total and average layoffs across industries, locations, and company stages.
    
    Examine layoff trends over time using visualizations.
     
    Identify industries and companies most affected by layoffs.
    
    Explore the relationship between funding raised and employee layoffs.
    
    Compare company size before and after layoffs to assess impact.
    
    Calculate and visualize layoff percentages across various dimensions.
    
## 📊 Key Visualizations
### Total laid off

<img width="258" height="138" alt="Screenshot 2025-07-19 184818" src="https://github.com/user-attachments/assets/b9e463a5-9f1b-420d-8053-bc0d9f64dab6" />

### Average laid off

<img width="248" height="131" alt="Screenshot 2025-07-19 184836" src="https://github.com/user-attachments/assets/946797d9-df7a-481d-97fe-1f732b0a83c5" />

### Total money raise

<img width="374" height="125" alt="Screenshot 2025-07-19 184844" src="https://github.com/user-attachments/assets/89059b85-5b0f-4330-8d1a-4f3bc486d9de" />

### Average money raise

<img width="399" height="130" alt="Screenshot 2025-07-19 184852" src="https://github.com/user-attachments/assets/0e86e185-8bb0-46e5-b458-76b3bc8a854e" />

### Laid off by location

<img width="845" height="702" alt="Screenshot 2025-07-19 184957" src="https://github.com/user-attachments/assets/46eda5b7-a45c-4232-ae5d-14f5bb2c2b8c" />

### Laid off as per company

<img width="862" height="669" alt="Screenshot 2025-07-19 185027" src="https://github.com/user-attachments/assets/7133832a-652c-435e-960f-88f5f039e5f6" />

### Laid off as per year

<img width="791" height="584" alt="Screenshot 2025-07-19 185041" src="https://github.com/user-attachments/assets/1393933f-287d-4bf0-98fd-ca37e951d157" />

### Laid off as per industry

<img width="563" height="475" alt="Screenshot 2025-07-19 185100" src="https://github.com/user-attachments/assets/30d605d7-dd87-48de-aabf-68aa783a97ab" />

## 🛠️ Data Transformation using pandas library in python

### 🟢 Step 1: Establishing a Connection to the Database
    Established a connection between MySQL and Python (Pandas) to extract employee laid off data directly from the database.

    Used libraries like mysql-connector-python

    Executed SQL queries to fetch data into Python for further analysis.

#### 🟢 Step 2: convert data into DataFrame using pandas(Python)
    loaded the extracted data into python for pre processing.

#### 🟢 Step 3: Data understanding and quality check
    Explored the structure of the dataset.

    Checked column data types, null values, column quality, and column distribution to understand the data.

#### 🟢 Step 4: Data Cleaning & Transformation

    Removed null values and duplicate rows
    
    Renamed columns for clarity
    
    Changed data types (e.g., date, integer, float) appropriately 

    Removes unwanted columns
    
    Reorganized into a clean tabular format for better analysis

#### 🟢 Step 5: Doing Explotary Data Analysis

    create KPis for EDA like total churn, total customer, churn rate etc. and 

    Generated insightful visualizations using Matplotlib

    Total and averge laid off

    laid off rates
     
#### 🟢 Step 6: Export cleaned data for visualization

    After doing EDA the clean dataset export to an excel(.xlsx) file format using pandas and load into power BI for visualization.

## 🛠 Tools & Technologies
    Pyhton (pandas, numpy, matplotlib)

    Jupyter Notebook

    MySQL

    Power Bi
    
    DAX Measures
    
## 📌 DAX Highlights
    Total_Laid_off = sum(Sheet1[Laid_Off])

    Average_Laid_off = Average(Sheet1[Laid_Off])

    Total_money_raised = sum(Sheet1[Money_Raised_in_mil])

    Average_money_raised = Average(Sheet1[Money_Raised_in_mil])
    
    Laid_off_rate = (sum(Sheet1[Laid_Off])/sum(Sheet1[Company_Size_before_Layoffs]))*100

## 💡 Insights Uncovered
    Total Layoffs: 27,000 employees laid off across multiple companies.
    
    Average Layoffs per Entry**: 253.06  
    
    Layoff Rate: 10.10% (Laid off compared to total pre-layoff workforce)
    
    Total Money Raised: $8 Million  
    
    Average Money Raised: $76.18K
    
 ## 📬 Contact / Credits
Author: Ajit Kumar Samal

LinkedIn: www.linkedin.com/in/ajitkumarsamal

GitHub: https://github.com/Ajit805-lab

Email: ajitkumarofficial79@gmail.com


    



