# Black Friday Purchases Analysis

## Overview
This project aims to analyze customer purchase behavior during Black Friday sales, specifically focusing on how purchase amounts correlate with various customer demographics and other factors. The insights derived from this analysis can help the management team make informed business decisions regarding marketing strategies, product placements, and inventory management.

## Dataset
The analysis utilizes transactional data collected from customers who purchased products during Black Friday. The dataset, `sales_data.csv`, includes the following features:

* **User_ID**: Unique identifier for each customer.
* **Product_ID**: Unique identifier for each product.
* **Gender**: Sex of the customer (Male/Female).
* **Age**: Age of the customer, categorized into bins (e.g., 0-17, 18-25, 26-35, 36-45, 46-50, 51-55, 55+).
* **Occupation (masked)**: Anonymized occupation category for the customer.
* **City_Category**: The category of the city where the customer resides (A, B, or C).
* **Stay_In_Current_City_Years**: Number of years a customer has resided in their current city.
* **Marital_Status**: Marital status of the customer (0 for unmarried, 1 for married).
* **Product_Category (masked)**: Anonymized product category.
* **Purchase**: The purchase amount (target variable).

The dataset contains 550,068 entries and 10 columns, with no missing or duplicate values found during initial exploration.

## Analysis & Key Insights

The analysis involved comprehensive data exploration, cleaning, and visualization to uncover patterns in customer spending behavior. Key insights include:

* **Gender-Based Spending**: Male consumers contributed significantly more to the total purchase value compared to female consumers.
* **Age Group Contributions**:
    * The **26-35** age group was the highest contributor to overall sales.
    * Following closely were the **36-45** and **18-25** age groups.
    * The **55+** and **0-17** age groups, despite lower total sales, exhibited the highest average purchase values, suggesting they tend to make fewer but larger purchases.
* **Marital Status and Spending**: Unmarried customers displayed more active spending habits compared to married customers.
* **City-Based Purchase Behavior**:
    * **City B** recorded the highest total purchases, followed by City C and City A.
    * **City A** and **City B** had the highest average transaction values.
    * **City C** showed a higher number of smaller purchases.
* **Purchase Skewness**: The `Purchase` column exhibited moderate right-skewness, indicating a higher frequency of lower-value purchases.
* **Product Category Skewness**: `Product_Category` was highly right-skewed, suggesting that most purchases originate from a limited number of categories.

### Final Takeaways:
* Male consumers and the 26-35 age group are dominant contributors to Black Friday sales.
* Unmarried individuals and consumers in City B showed the highest total spending.
* The 55+ age group and City C, despite lower total sales, present notable average purchase values, highlighting opportunities for targeted strategies across different consumer groups.

## Technologies Used
* Python
* Pandas (for data manipulation and analysis)
* NumPy (for numerical operations)
* Matplotlib (for data visualization)
* Seaborn (for enhanced data visualization)

## Project Structure
``` bash
.
├── datasets
│   └── sales_data.csv
├── Notebooks
│   └── Black_Friday_Analysis.ipynb
├── README.md
└── requirements.txt
```