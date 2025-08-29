# Market Basket Analysis using Power BI
This project demonstrates how to perform Market Basket Analysis (MBA) using Power BI to uncover product purchase patterns. The technique is widely used in both brick-and-mortar retail and e-commerce for cross-selling, product recommendation, promotional bundling, and store layout optimization.

# Dataset
The dataset used is the Groceries Market Basket Dataset, containing transaction records where each row represents a set of products purchased together.
[click here](https://www.kaggle.com/datasets/irfanasrullah/groceries/data) to download the data set

# Key Concept
Market Basket Analysis is based on three main metrics:

- **Support** → How frequently two products appear together in transactions.
- **Confidence** → The likelihood of buying product B when product A is purchased.
- **Lift** → The strength of the relationship between two products compared to random chance.

Example:

Strawberry + Whipped Cream → Lift = 2
→ This means they are **twice as likely** to be purchased together than randomly.

# Analysis Steps
Data Preparation

- Load dataset into Power BI
- Transform with Power Query (Index column, Unpivot, Data cleaning, etc.)
- Final dataset in long format

Data Analysis
- Calculate total transactions and unique products with **DAX Measures**
- Generate product pairs using **CROSSJOIN**
- Compute **Support, Confidence, and Lift** with DAX

Data Visualization
- **Network Graph** → shows strong product associations (Lift-based)
- **Scatter Plot** → plots Support vs Lift
- **Matrix** → table with Support, Confidence, Lift values
- **KPI Cards** → highlight key metrics (total transactions, product count)

# Key Results
Some of the strongest product associations include:

- Root Vegetables ↔ Herbs → Lift: 3.96
- Whipped/Sour Cream ↔ Berries → Lift: 3.80
- Napkins ↔ Hygiene Articles → Lift: 3.54
- Frozen Vegetables ↔ Chicken → Lift: 3.25

These insights highlight product combinations useful for **promotions**, **recommendations**, and **marketing strategies**.

# Business Applications

- **Retail Stores** → Place frequently bought-together products near each other.
- **E-commerce** → Power recommendation engines (“Customers who bought this also bought…”).
- **Promotions & Bundling** → Create bundle discounts (e.g., frozen vegetables + chicken).

# Tools & Technologies

- **Power BI** for data visualization and reporting
- **DAX** for calculating Support, Confidence, and Lift
- **Power Query** for data transformation

# How to Run
1. clone this repository
<pre> git clone https://github.com/nrevanda/Market-Basket-Analysis-using-Power-BI </pre>

2. Open the **.pbix** file in Power BI Desktop
3. Follow the guide and analysis steps desribed in this guide
4. Explore the interactive dashboard

# Notes
- The Groceries dataset is included in this repository.
- Visualization thresholds can be adjusted (e.g., Lift > 2.2, Support > 0.6%).

