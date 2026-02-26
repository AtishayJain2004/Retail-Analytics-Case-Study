📊 Retail Analytics Case Study — Customer & Sales Analysis

This project analyzes retail customer behavior, product performance, and sales trends using Python and pandas. It is based on a multi-table retail dataset that includes customer information, transaction history, and product hierarchy details. The goal is to generate business insights by merging datasets, performing exploratory data analysis (EDA), and answering key retail intelligence questions.

🔍 Project Overview

Retail companies generate massive amounts of customer and transaction data.
This project demonstrates how to:

Clean and prepare real-world retail datasets

Merge multiple tables into a single analytical dataset

Handle mixed date formats, missing values, and negative transactions

Perform exploratory data analysis (EDA)

Identify sales patterns and customer trends

Answer business questions related to product popularity, store performance, and customer demographics

📁 Dataset Description

The project uses three primary datasets:

1. Customer.csv

Contains customer demographic information:

Customer ID

Gender

City code

Date of birth

Other personal details

2. Transactions.csv

Includes all customer transactions:

Transaction ID

Transaction date

Customer ID

Product category codes

Quantity

Total amount (returns are negative values)

3. prod_cat_info.csv

Contains product hierarchy:

Product category

Sub-category

Category codes for merging

🛠 Data Preparation & Merging

Three datasets were merged into a single dataframe Customer_Final using:

Key fields like cust_id, prod_cat_code, and prod_subcat_code

Correct join types (inner for customers with transactions, left for product info)

Date cleaning with pd.to_datetime()

Handling negative and invalid transactions

Adding derived metrics such as customer age

📈 Key Analysis Performed

The case study required answering major retail analytics questions, including:

✔ Summary statistics

Data types

Top & bottom observations

Five-number summary

Frequency distributions

✔ Transaction insights

Total number of negative transactions

Time period of available data

✔ Customer insights

Most popular categories among males vs females

Customers with more than 10 unique transactions

Age-based spending analysis (25–35 years)

✔ Store performance

Store types with highest sales (value & quantity)

✔ Product performance

Revenue from Electronics & Clothing in flagship stores

Revenue from male customers in Electronics

📉 Visualizations

The analysis includes:

Histograms for numerical variables

Bar charts for categorical variables

Category-wise comparisons

Customer & store performance trends

🧠 Key Insights & Outcomes

Electronics and Clothing were among the top-performing categories

Flagship stores contributed the highest revenue

City-level analysis revealed customer concentration across different regions

The 25–35 age group showed strong purchasing activity

Female and male customers differed in category preferences

Returns (negative transactions) impacted the net revenue

Clean merging of datasets enabled complete retail intelligence

🧰 Technologies Used

Python

Pandas

NumPy

Matplotlib

Jupyter Notebook

📂 Project Structure
Retail-Analytics-Case-Study/
│
├── data/
│   ├── Customer.csv
│   ├── Transactions.csv
│   ├── prod_cat_info.csv
│
├── notebooks/
│   ├── Retail_Case_Study.ipynb
│
├── README.md
└── requirements.txt
🚀 How to Run

Clone the repository:

git clone https://github.com/<your-username>/Retail-Analytics-Case-Study.git

Install dependencies:

pip install -r requirements.txt

Open the notebook:

jupyter notebook

Run the cells to reproduce the analysis.

⭐ What I Learned

End-to-end data cleaning and preprocessing

Dataset merging and relational analysis

Exploratory data analysis techniques

Retail-specific KPIs and insights

Handling messy, real-world data

Data storytelling for business decision-making
