# COMPREHENSIVE EXPLORATORY DATA ANALYSIS OF CUSTOMER DEMOGRAPHICS AND SPENDING BEHAVIOR

This project presents a comprehensive exploratory data analysis (EDA) of customer data, aiming to provide insights into customer demographics, spending patterns, and campaign effectiveness.

# Project Overview 

The main goal of this EDA is to analyze a dataset containing customer information and their spending habits. By identifying patterns, managing outliers, and performing feature engineering, this analysis offers key insights into customer behavior, which can be used for targeted marketing strategies, product optimization, and campaign improvement.

# Dataset Description
The dataset used for this analysis contains various customer-specific attributes, including:

+ ID: Unique identifier for each customer.
+ Year_Birth: The birth year of the customer.
+ Education: The customer's education level.
+ Marital_Status: The customer's marital status.
+ Income: The annual income of the customer.
+ Kidhome: The number of children living at home.
## Spending columns: Various spending categories, including:
+ MntWines
+ MntFruits
+ MntMeatProducts
+ MntFishProducts
+ MntSweetProducts
+ MntGoldProds
# Key Features of the EDA
## 1. Data Cleaning and Preprocessing
+ Missing Values: Missing values in the income column were filled based on the mean income for each education level.
+ Data Type Correction: The Income column was converted from an object to a float, and the Dt_Customer (customer registration date) was converted to datetime format.
Outlier Handling: Outliers in key columns such as Income and Year_Birth were capped using the interquartile range (IQR) method to ensure robust analysis.
## 2. Feature Engineering
+ Age Calculation: A new Age column was created by subtracting Year_Birth from the current year.
+ Total Amount Spent: A new TotalAmount_Spent column was created by summing spending across all product categories.
+ Total Purchases: A new Total_Purchases column was created by summing the number of purchases from different channels.
+ Campaign Acceptance: A TotalCampaignsAcc column was created to track the number of campaigns accepted by each customer.
## 3. Exploratory Data Analysis (EDA)
## Univariate Analysis
+ Income Distribution: Analysis of the distribution of customer income.
+ Age Distribution: Exploration of the age demographics of customers.
## Bivariate Analysis
+ Income vs Total Amount Spent: Examined the relationship between income and total spending across product categories.
+ Income vs Education: Investigated how education level correlates with income levels.
## 4. Marketing Campaign Analysis
+ Campaign Success: Assessed the effectiveness of marketing campaigns by analyzing acceptance rates across campaigns.
+ Product Performance: Analyzed spending behavior by product category and age group to identify high-revenue products and potential opportunities for growth.
# Key Findings
+ Age Distribution: The majority of customers fall within a specific age range, which can guide targeted marketing efforts.
+ Spending Patterns: A positive correlation between income and spending was observed, with higher-income customers spending more across all product categories.
+ Marketing Campaign Success: Campaign 5 showed the highest success rate, suggesting that future campaigns could follow its structure.
+ Product Performance: High-revenue products, such as wines and meats, were identified as key areas for marketing focus.
# Recommendations
+ Targeted Campaigns: Focus future marketing efforts on customer segments with higher campaign acceptance rates.
+ Product Optimization: Allocate resources to promote high-revenue products, while devising strategies to boost sales for lower-performing categories.
+ Customer Segmentation: Segment customers by age and tailor marketing messages. Older customers tend to spend more, and premium products may resonate with this demographic.
# Installation and Usage

## Clone the repository:
+ bash
+ Copy code
+ git clone https://github.com/your-username/EDA-Customer-Demographics.git
## Install the required libraries:

+ bash
+ Copy code
+ pip install -r requirements.txt
## Run the notebook:

Open the Jupyter notebook file (EDA Project.ipynb) in your preferred environment and follow along with the code for detailed analysis.

## Libraries Used
+ pandas
+ numpy
+ matplotlib
+ seaborn
# Conclusion
This exploratory data analysis provides actionable insights into customer demographics, spending behavior, and campaign performance. The findings support the development of data-driven marketing strategies and suggest further avenues for predictive analysis.
