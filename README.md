#  Retail Sales Data Analysis (Python – Pandas, Matplotlib)

This project explores a real-world style retail dataset and demonstrates a complete data analysis workflow, including data cleaning, exploratory data analysis (EDA), customer insights, and business-driven interpretations.

The notebook walks through the process step by step — from handling missing values to generating visual insights and applying customer lifetime value (CLV) logic.

---

##  Project Objectives

- Clean and prepare a dataset containing missing and inconsistent values  
- Analyze sales performance across product categories  
- Evaluate the impact of discount usage on customer spending behavior  
- Identify high-value customers using **Customer Lifetime Value (CLV)** logic  
- Explore repeat-customer behavior in a SaaS-style retention approach  

---

##  Data Cleaning Steps

| Step | Description |
|-------|-------------|
| Missing values detected using `.isna()` |
| Imputed missing *Item* values with `"Unknown"` |
| Filled missing *Price Per Unit* using **category-level averages**  |
| Computed missing *Total Spent* from `Price Per Unit × Quantity` |
| Handled missing *Discount Applied* values and fixed dtype  |
| Verified dataset is fully clean (`df.isna().sum() == 0`)  |

---

##  Exploratory Analysis (EDA)

 **Category-level revenue & quantity analysis**  
 **Discount effect on average spending and transaction count**  
 **Boxplot comparison of spending with vs without discount**  
 **Top customers by total revenue (CLV approach)**  
 **Repeat-customer analysis (0 one-time customers detected)**

---

##  Key Insights

- **Butchers, Electric Household Essentials, and Beverages** are the highest-revenue categories  
- Discounts **do not increase spending per order**, but do reduce full-price transactions  
- The **top 10 customers contribute ~40% of total revenue**, showing high customer concentration  
- All customers in the dataset are **repeat customers (100% retention)**  
- Revenue is heavily driven by loyal, high-frequency buyers — retention > acquisition in this scenario  

---

##  Tech Stack

| Tool | Purpose |
|-------|---------|
| Python | Main analysis |
| Pandas | Data wrangling, aggregations |
| NumPy | Calculations, numeric ops |
| Matplotlib | Visualizations |
| Jupyter Notebook | Analysis environment |

---

##  Usage

You can open the `.ipynb` notebook directly in Jupyter Notebook, JupyterLab, or Google Colab.  
No additional setup is required other than having Python with Pandas, NumPy, and Matplotlib installed.
