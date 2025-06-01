# **Data Cleaning Project**  

## **📌 Project Overview**  
This project focuses on cleaning a dataset containing over 50,000 rows of data using Excel, Power Query, Power Pivot, PostgreSQL, and Python to ensure accuracy, consistency, and usability. The dataset requires **multiple preprocessing techniques**, including handling **duplicates, inconsistent values, white spaces, and missing data**.  

### **0️⃣ Data structure overview**  
- Conduct an initial data exploration to understand its structure, variables, and quality.  
- Identify potential issues that may impact the analysis.  
- **Check for columns with short or inconsistent values**, such as:  
  - **S** for *Single*, **M** for *Married*  
  - **F** for *Female*, **M** for *Male*  

### **1️⃣ Executive Summary**  
- Using Power Query, Power Pivot, and Excel functions to identify and remove duplicate records efficiently.  
- Leveraging **Power Pivots aggregations** to detect duplicate patterns and inconsistencies.  
- Using PostgreSQL’s WINDOW function `ROW_NUMBER` to detect duplicate records in structured data.  
- Using Python’s `duplicated()` function to find and remove duplicate rows in Pandas:
- 
### **2️⃣ Insights deep dive**  
- Identify missing entries using **Excel formulas**, **Power Query transformations**, and **SQL queries**.  
- Apply Python functions such as:  

### **3️⃣ Recommendations**  
- Standardize categorical variables using consistent labels and encoding.  
- Apply PostgreSQL transformations and Python's Pandas for categorical adjustments. 

## **🚀 Next Steps**  
- Conduct exploratory data analysis (EDA) after cleaning.  
- Create visualizations using Excel Charts, Tableau, and Python with Matplotlib and/or Seaborn libraries.  
- Prepare cleaned data for business use, such as reporting, forecasting, or visualization. 
