# **Data Cleaning Project**  

## **📌 Project Overview**  
This project focuses on cleaning a dataset containing over 50,000 rows of data using Excel, Power Query, Power Pivot, PostgreSQL, and Python to ensure accuracy, consistency, and usability. The dataset requires **multiple preprocessing techniques**, including handling **duplicates, inconsistent values, white spaces, and missing data**.  

## **🎯 Objectives**  
Improve data quality by detecting and correcting **duplicates, inconsistent values, white spaces, and missing data**. Prepare data for **exploratory data analysis** and further business use.  

## **🛠️ Tools & Technologies**  
- Excel, Power Query & Power Pivots (Data transformation & cleaning)  
- PostgreSQL (Database validation & structured queries)  
- Python (Pandas, for Numpy and OS for automation & additional cleaning)  

## **📑 Data Cleaning Process**  

### **0️⃣ Dataset initial review**  
- Conduct an initial data exploration to understand its structure, variables, and quality.  
- Identify potential issues that may impact the analysis.  
- **Check for columns with short or inconsistent values**, such as:  
  - **S** for *Single*, **M** for *Married*  
  - **F** for *Female*, **M** for *Male*  

### **1️⃣ Detect Duplicate Rows**  
- Using Power Query, Power Pivot, and Excel functions to identify and remove duplicate records efficiently.  
- Leveraging **Power Pivots aggregations** to detect duplicate patterns and inconsistencies.  
- Using PostgreSQL’s WINDOW function `ROW_NUMBER` to detect duplicate records in structured data.  
- Using Python’s `duplicated()` function to find and remove duplicate rows in Pandas:  

  ```python
  import pandas as pd
  df = pd.read_csv("data.csv")
  duplicates = df[df.duplicated()]
  df_cleaned = df.drop_duplicates()
  ```

### **2️⃣ Detect Missing Values**  
- Identify missing entries using **Excel formulas**, **Power Query transformations**, and **SQL queries**.  
- Apply Python functions such as:  

  ```python
  df.isna().sum()
  df.isnull().sum()
  df["column_name"].value_counts()
  df["column_name"].unique()
  ```

### **3️⃣ Re-Express Categorical Variables**  
- Standardize categorical variables using consistent labels and encoding.  
- Apply PostgreSQL transformations and Python's Pandas for categorical adjustments.  

### **4️⃣ Document Issues in Issue Log**  
- Maintain a structured issue log to track identified problems, resolutions, and methodology.  
- Ensure transparency in data cleaning decisions for **reproducibility**.  

## **📂 Project Structure**  

```
📂 data-cleaning-project  
 ├── 📁 raw-data/ *(Unprocessed dataset files)*  
 ├── 📁 cleaned-data/ *(Processed dataset files)*  
 ├── 📁 scripts/ *(Python & SQL scripts for cleaning)*  
 ├── 📁 documentation/ *(Documentation & findings)*  
 ├── README.md *(Project overview)*
```

## **🚀 Next Steps**  
- Conduct exploratory data analysis (EDA) after cleaning.  
- Create visualizations using Excel Charts, Tableau, and Python with Matplotlib and/or Seaborn libraries.  
- Prepare cleaned data for business use, such as reporting, forecasting, or visualization. 
