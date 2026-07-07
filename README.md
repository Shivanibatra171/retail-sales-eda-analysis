# 📊 Retail Sales – Exploratory Data Analysis

## 📌 Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on a retail sales dataset to uncover patterns in customer behavior, product performance, and sales trends. The analysis includes data cleaning, statistical exploration, and visualization to generate actionable business insights.

This project was completed as part of a Data Science Internship (Task 1: Exploratory Data Analysis).

---

## 📂 Dataset
- **Source:** [Kaggle – Retail Sales Dataset](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset)
- **Records:** 1,000 transactions
- **Features:** Transaction ID, Date, Customer ID, Gender, Age, Product Category, Quantity, Price per Unit, Total Amount
- **Product Categories:** Beauty, Clothing, Electronics

---

## 🛠️ Tools & Libraries Used
- Python 3
- Pandas – data manipulation and cleaning
- NumPy – numerical operations
- Matplotlib & Seaborn – data visualization
- Jupyter Notebook – analysis environment

---

## 🧹 Data Cleaning Steps
- Removed duplicate transaction records
- Checked and handled missing values
- Converted `Date` column to proper datetime format
- Created derived features: `Month` (for trend analysis) and `Age Group` (for demographic analysis)
- Used boxplots to detect and evaluate outliers in `Total Amount`

---

## 🔍 Key Insights
- **Electronics** is the top revenue-generating category (~157,000), closely followed by **Clothing** (~156,000), with **Beauty** slightly lower (~144,000)
- Sales are almost evenly split by gender: **51.1% Female** vs **48.9% Male**
- Customer age is fairly evenly distributed between 20–64 years, with no dominant age group
- **May 2023** was the peak sales month (~53,000); **September 2023** was the lowest (~24,000)
- **Price per Unit** has the strongest correlation with Total Amount (**0.85**), making it the key driver of transaction value
- Quantity has a moderate correlation with sales (0.37), while Age has almost no impact (-0.06)

---

## 📈 Visualizations
This project includes the following charts (available in the `/screenshots` folder):

| Chart | Description |
|---|---|
| Bar Chart | Total Sales by Product Category |
| Line Chart | Monthly Sales Trend |
| Histogram | Age Distribution of Customers |
| Correlation Heatmap | Relationship between Age, Quantity, Price, and Total Amount |
| Scatter Plot | Price per Unit vs Total Amount |
| Pie Chart | Sales Distribution by Gender |
| Box Plot | Outlier Detection in Total Amount |

---

## 💡 Business Recommendations
- Prioritize Electronics in inventory and marketing spend, as it drives the highest revenue and per-transaction value
- Keep marketing strategies broad/inclusive, since neither gender nor age strongly influences spending
- Run promotional campaigns during low-sales months (e.g., September) to stabilize monthly revenue
- Focus on increasing average price per unit (via bundling/upselling) rather than volume, since price is the biggest driver of sales value

---

## 📁 Repository Structure

retail-sales-eda-analysis/

├── EDA_Retail_Sales.ipynb        # Complete Jupyter Notebook with code & analysis

├── retail_sales_dataset.csv      # Cleaned dataset

├── EDA_Report.pdf                # Full analysis report

├── screenshots/                  # Chart images

└── README.md                     # Project documentation
