# TelecomCustomerChurn

## Project Objective

This project analyzes Telecom Customer Churn data for visualization and data analysis, we will explore factors of who are high-risk churn customers and what sort of behavior/ preferences are associated with them. 

## Objectives

The primary objectives of this project are:

1. Identify High-Value Customers:
   - Analyze demographics, tenure, and pricing plans to determine characteristics of low-churn customers.

2. Understand Churn Behavior:
   - Investigate behaviors and preferences associated with high churn rate customers, focusing on contract types, streaming usage, payment methods, and data protection measures.
   - Identify trends in customer behavior that correlate with increased churn.

3. Generate Retention Strategies:
   - Develop actionable recommendations for reducing churn based on insights gathered from high-value and high-risk customer behaviors.

## Repository Structure

**Dataset**
- Contains the original WA_Fn-UseC_-Telco-Customer-Churn.csv and the new cleaned / processed datasets telo_customerchurn.csv

**Preprocessing** (TeleCustomerChurn.ipynb)
- Contains a Python notebook to clean, process for analysis and visualization

**Visualization** (TelecomCustomerChurn.twb)
- Contains a Tableau workbook file featuring visualizations, and two dashboards to address project objectives
  
## Data Preprocessing 

The dataset was cleaned with Python to convert certain data column into the correct data type (such as object to numeric). Missing values were filled with the mean value. Certain column's data was mapped to values that would allow for more intuitive visualizations, such as 0 and 1 to No and Yes.

## Tableau Visualizations

Visit the [Tableau Dashboard](https://public.tableau.com/app/profile/melody.feng/viz/TelecomCustomerChurn_17300808484380/ChurnCTLFactors#1)to explore the visualizations and insights.

## Key Questions and Insights

### 1. Who are high-value customers that are less likely to churn?

Analysis: I explored the type of customers who churnend and did not churn, such as their demographics, the tenure and pricing plan they selected and the plan services regarding Internet and Phone Services.

Visualization: Dashboard made of visualizations including: Amount of customers who churned and did not churn (Bar Chart), Tenures and the amount of people per tenure who churned (Bubble Chart), Churn Rate per monthly charge (Line Graph), Partner and Dependent Churn Rates (Table), CLV of Phone Services Customer and Internet Services Customer (Bar Charts)

Insight: 
  - Demographics: Families— those with a partner and dependents—exhibit lower churn rates.
  - Tenure and Pricing: Customers who have been with the company for over two years and have monthly charges under $60 are also less likely to churn.
  - Plan Services: High Customer Lifetime Value (CLV) customers often have subscription plans that have Phone Service and Fiber Optic Internet.

<img width="982" alt="Screenshot 2024-10-27 at 9 37 21 PM" src="https://github.com/user-attachments/assets/ff4924e0-4b13-4f65-a208-68f36b0025ae">

### 2. When focusing on plan specifics, what behaviors characterize high churn rate customers?

Analysis: I compared behaviors associated with high churn rate customers, looking into their preferences in terms of phone plans such as contract type, streaming TV or movies, payment method, paperless billing and online protections. 

Visualization: Contract Type Churn Rate (Highlight Table), Streaming TV and Movie Churning Churn Rate (Stacked Bar Chart), Payment Method Churn Rate (Bar Chart), Paperless Billing Churn Rate (Bar Chart), Online Secuirty, Backup and Device Protection (Highlight Table)

Insight: 
  - Contract Type: Month-to-month contracts exhibit the highest churn rates.
  - Internet Plans: Among month-to-month contracts, customers with Internet plans who do not stream TV or movies also show a significant propensity to churn.
  - Payment Methods: Customers who opt for paperless billing and pay via electronic checks experience higher churn rates compared to those who use automatic bank transfers or credit card auto-pay.
  - Data Protection: Customers who take proactive measures to protect their data—such as setting up online security, backups, and device protection—demonstrate significantly lower churn rates, indicating that their investments in security lead to greater retention.

<img width="983" alt="Screenshot 2024-10-27 at 9 37 31 PM" src="https://github.com/user-attachments/assets/f8abbef8-d763-45e6-adda-aea5c903fe61">

## Conclusion and Recomendations 

Based on the insights from this analysis, as a telecom provider it is valuable to consider:

**1. Target High-Value Customer Segments:** Focus marketing and retention efforts on families, long-tenured customers to minimize churn.

**2. Revise Contract Offerings:** Reevaluate the month-to-month contract options, as they show the highest churn rates. Consider incentivizing longer-term commitments with benefits that enhance customer loyalty.

**3. Enhance Service Bundling:** Promote bundled offerings that include Phone Service and Fiber Optic Internet, as these attract customers with high Customer Lifetime Value (CLV).

**4. Improve Customer Engagement:** Implement initiatives that encourage proactive customer behaviors, such as setting up online security and device protection, to enhance retention rates among high-risk groups.

## Dataset

The dataset used in this analysis was scraped from IBM comprising of 7043 rows.  

### Key Attributes:

- **Customer Data:** customerID, gender, SeniorCitizen, Partner, Dependents, Churn
- **Contract Data:** tenure, Contract
- **Plan Data:** PhoneService, MultipleLines, InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies,  
- **Billing Data:** PaperlessBilling, PaymentMethod, MonthlyCharges, TotalCharges

This project uses Telecom data sourced from [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data).
