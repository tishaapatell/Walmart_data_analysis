**Walmart Sales & Profitability Analysis** 

📌** Project Overview **

This project analyzes Walmart’s sales dataset to uncover trends, patterns, and profitability insights across different product categories, locations, and customer behaviors. The goal is to provide data-driven recommendations that can support decision-making in inventory management, pricing strategy, and marketing campaigns. 



⚙** Environment Setup **

**1. Tools Used **

• **Visual Studio Code \(VS Code\)** – Development environment 

• **Python 3.8\+** – Data analysis and processing 

• **SQL Databases:** MySQL, PostgreSQL – For structured data storage and SQL analysis **Goal:** Create a structured workspace in VS Code and organize project folders for smooth development and data handling. 



**2. Set Up Kaggle API **

• **Obtain API Key:** Download your kaggle.json file from Kaggle API settings under your profile. 

• **Configure:** Place kaggle.json in your local .kaggle/ folder. 

• **Download Dataset:** 

kaggle datasets download -d <dataset-path> 

• **Storage:** Save datasets in the data/ folder for easy reference. 



**3. Download Walmart Sales Data **

• **Data Source:** Kaggle – Walmart Sales Dataset 

• Save files to data/ directory. 



**4. Install Required Libraries** pip install pandas numpy sqlalchemy mysql-connector-python psycopg2 

**Libraries Used:** 

• pandas – Data manipulation 

• numpy – Numerical computations 

• sqlalchemy – Database connections 

• mysql-connector-python – MySQL integration 

• psycopg2 – PostgreSQL integration **5. Explore the Data **

• Load CSV into a Pandas DataFrame: import pandas as pd 

df = pd.read\_csv\('data/walmart\_sales.csv'\) df.info\(\) 

df.describe\(\) 

df.head\(\) 

• Check distribution, column names, types, and potential issues. 



**6. Data Cleaning **

• Remove duplicates 

• Handle missing values 

• Fix data types \(dates → datetime, prices → float\) 

• Format currency 

• Validate cleaned data 



**7. Feature Engineering **

• Create Total Amount column: 

df\['Total\_Amount'\] = df\['Unit\_Price'\] \* df\['Quantity'\] 

• This helps in faster aggregation during SQL queries. 





**8. Load Data into SQL Databases **

• Connect to MySQL & PostgreSQL via SQLAlchemy 

• Automate table creation and data insertion 

• Verify with initial SQL queries **9. SQL Analysis **

Key business questions answered: 

• Revenue trends across branches & categories 

• Best-selling product categories 

• Sales performance by time, city, and payment method 

• Peak sales periods 

• Profit margin analysis by branch and category **10. Project Publishing **

• Document the workflow in: 

o README.md \(this file\) 

o Jupyter Notebooks 

o SQL scripts 

• Push to GitHub with: 

o Code files 

o Data \(if allowed\) or data access instructions o Visualizations 



📊** Key Insights **

• **Sales:** Highest sales in \[Top Category\] and \[Top Branch\] 

• **Profitability:** \[Top Category\] yields maximum profit 

• **Customer Trends:** Peak hours identified for targeted promotions 



🚀** Future Enhancements **

• Add real-time dashboards in Power BI/Tableau 



• Automate data ingestion & analysis 

• Incorporate external datasets for deeper insights 



📜** Acknowledgments **

• **Data Source:** Kaggle – Walmart Sales Dataset 

• **Inspiration:** Walmart’s business case studies on sales & supply chain



