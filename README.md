# SQL Portfolio Project Repository

Welcome to my SQL Portfolio Project repository! This repository showcases my SQL skills through various projects, including data cleaning and exploratory data analysis (EDA). Below, you'll find an overview of the projects included, the objectives they aim to achieve, and the SQL techniques demonstrated.

---

## Repository Description
This repository contains SQL scripts and related materials for portfolio projects aimed at solving real-world data challenges. The goal is to demonstrate proficiency in SQL by performing data cleaning, analyzing trends, and extracting insights from datasets. The projects use a dataset from Kaggle on layoffs in 2022 ([Link to Dataset](https://www.kaggle.com/datasets/swaptr/layoffs-2022)).

---

## Projects

### 1. Data Cleaning

**Objective:**  
Clean and prepare the raw dataset for analysis by addressing duplicates, standardizing data, handling null values, and removing unnecessary rows and columns.

**Techniques Used:**  
- **Removing duplicates** using `ROW_NUMBER()` and `WITH` Common Table Expressions (CTEs).  
- **Standardizing data:** Fixing inconsistent values (e.g., industry names and country formats) and updating blank values to `NULL`.  
- **Handling null values:** Populating null fields where possible using data from similar records.  
- **Column transformations:** Converting text fields to appropriate data types (e.g., `DATE` conversion using `STR_TO_DATE`).  
- **Deleting irrelevant data:** Identifying and removing records with insufficient information.  

**SQL Highlights:**  
- Dynamic updates for filling missing data.  
- Consistent formatting for categorical values.  
- Application of SQL functions like `TRIM`, `ROW_NUMBER`, and `STR_TO_DATE`.

---

### 2. Exploratory Data Analysis (EDA)

**Objective:**  
Explore the cleaned dataset to uncover insights, trends, and patterns related to layoffs in 2022.

**Techniques Used:**  
- Aggregation using `GROUP BY` to analyze trends by:
  - Company
  - Location
  - Country
  - Industry
  - Funding stage  
- Ranking with `DENSE_RANK()` to identify top companies for layoffs per year.  
- Rolling totals using `OVER` window functions to track cumulative layoffs over time.  

**SQL Highlights:**  
- Identification of companies with the highest layoffs overall and by year.  
- Insights into layoffs by industry and location.  
- Visualization-ready summaries for further analysis.

---

## Folder Structure
- **/data**: Contains sample data (if applicable).  
- **/scripts**: SQL scripts for each project.  
  - `data_cleaning.sql`: SQL code for cleaning the dataset.  
  - `eda.sql`: SQL code for exploratory data analysis.  
- **/outputs**: Contains any exported results or visualizations derived from SQL queries.

---

## Tools Used
- **SQL Engine**: MySQL (compatible with most relational database systems).  
- **Dataset Source**: Kaggle ([Layoffs 2022](https://www.kaggle.com/datasets/swaptr/layoffs-2022)).

---

## How to Use
1. Clone the repository: `git clone https://github.com/yourusername/sql-portfolio-projects.git`.  
2. Set up the database:
   - Load the dataset into your preferred SQL database.
   - Run the scripts in the `/scripts` folder.  
3. Explore the insights:
   - Use the queries in `eda.sql` to uncover trends and visualize data.

---

## Key Takeaways
This repository highlights my ability to:
- Transform raw data into clean and structured formats.  
- Perform advanced SQL operations to extract actionable insights.  
- Present meaningful trends and patterns for decision-making.  

Feel free to explore the repository, run the queries, and reach out if you have any questions or suggestions. Happy querying!
