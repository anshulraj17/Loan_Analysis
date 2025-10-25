#  Loan Data Analysis Dashboard
(Link: http://bit.ly/479oaRC)

###  Advanced Dashboard Development for Loan Data Analysis  
A comprehensive Power BI project providing a detailed view of lending operations, borrower behavior, and loan performance metrics.

---

##  Project Overview

This project presents a **Loan Data Analysis Dashboard** built in **Power BI** using the `Loan_dataset.csv` dataset.  
It provides deep insights into loan performance, funding patterns, and bad-loan behavior across multiple dimensions such as **time, geography, purpose, and borrower profile**.

---

##  Dashboard Pages

### **1. Home Page – Loan Performance Summary**
This dashboard highlights overall loan portfolio performance and funding trends.

#### **Key Visuals & Insights**
- **Funded Amount Over Time** – Month-wise trend analysis  
- **Funded Amount by State** – Geographical heatmap of loan distribution  
- **Funded Amount by Purpose** – Loan utilization analysis  
- **Loan Applications by Employee Length** – Borrower experience segmentation  
- **Funded Amount by Loan Status** – Fully paid vs charged-off vs current loans  

---

### **2. Bad Loan Summary**
This page dives deeper into **default analysis** and identifies key patterns behind bad loans.

#### **Key Visuals & Insights**
- **Bad Loan % by Month** – Monthly trend of defaults  
- **Bad Loans by Professional Experience** – Beginner | Mid-Level | Experienced  
- **Bad Loans by Purpose** – Purpose-wise default rate with average interest rate  
- **Bad Loans by Loan Term** – Comparison of 36 vs 60-month terms  
- **Bad Loans by State** – Top default-prone regions  
- **Bad Loan % by Grade** – Risk profile across loan grades  

---

##  Dataset Details

**File:** `Loan_dataset.csv`  
The dataset contains anonymized loan-level information, including:

- Loan amount, funded amount, and received amount  
- Loan purpose and grade  
- Borrower employment length and income  
- Interest rate and DTI (Debt-to-Income ratio)  
- Loan status (fully paid, charged off, current)  
- Issue date and state information  

Data was cleaned and transformed using **Power Query**, and key measures were created in **DAX**, including:

```DAX
Paid Loan % = DIVIDE([Paid Loans], [Total Loans])
Bad Loan % = DIVIDE([Charged-Off Loans], [Total Loans])
Average Interest Rate = AVERAGE(Loan[Interest Rate])
Average DTI = AVERAGE(Loan[DTI])
Average Funded Amount = AVERAGE(Loan[Funded Amount])

```

### Insights & Findings
 - California (CA) has the highest number of bad loans.

 - Small business loans show the highest bad-loan rate (~25%).

 - Default probability increases slightly for longer loan terms (60 months).

 - Beginner-level professionals contribute to a larger share of bad loans.

 - Average DTI remains consistent across good and bad loans (~0.13 – 0.14).

### Learning Outcomes
Through this project, the following analytical and technical skills were demonstrated:

- Data cleaning & modeling using Power Query

- DAX formula creation for KPIs and calculations

- Multi-page dashboard design with slicers and dynamic interactions

- Insight generation & business storytelling through visual analytics


### How to Use
- Clone or download this repository.

- Open the .pbix file in Power BI Desktop.

- Connect the dataset (Loan_dataset.csv).

- Explore both dashboards interactively using filters and slicers.


### Repository Structure

<img width="294" height="256" alt="image" src="https://github.com/user-attachments/assets/23a1a1aa-c2ce-4b18-8eb1-368784b5fb4e" />



