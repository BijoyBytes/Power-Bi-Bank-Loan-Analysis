# Financial Analysis – Bank Loan Performance – Power BI

## Project Overview

**Project Title:** Financial Analysis – Bank Loan Performance  
**Level:** Intermediate  
**Tool:** Microsoft Power BI  

This project focuses on analyzing bank loan performance using Power BI to monitor lending health, borrower behavior, and financial risk. Interactive dashboards help stakeholders track loan disbursement, repayment patterns, defaults, and key financial KPIs to support data-driven lending decisions.

![Library_project](https://github.com/BijoyBytes/Power-Bi-Bank-Loan-Analysis/blob/main/loan-performance-analysis-slide1.png)

## Objectives

- Analyze overall loan portfolio performance and growth trends.
- Track key KPIs such as Total Loan Amount, Interest Earned, Default Rate, and Recovery Rate.
- Identify high-risk loan segments based on borrower profile and loan type.
- Enable dynamic filtering by loan status, region, tenure, and borrower category.
- Provide actionable insights for risk management and credit strategy optimization.

## Project Structure

### 1. Data Sources & Preparation

* Used a single Excel file containing loan, borrower, and repayment details.
* Applied Power Query transformations:

  * Removed duplicates and invalid records.
  * Standardized date and currency formats.
  * Handled missing values and outliers.
  * Merged borrower and loan reference tables.
* Created calculated columns for loan tenure, EMI, and risk flags.


### 2. Data Model & Measures

* Built DAX measures to calculate KPIs:

```dax
• Total Loan Amount = SUM(fact_loans[Loan_Amount])  
• Total Repaid Amount = SUM(fact_repayments[Amount_Paid])  
• Outstanding Amount = Total Loan Amount – Total Repaid Amount  
• Default Rate = Defaulted Loans / Total Loans  
• Recovery Rate = Recovered Amount / Defaulted Amount  
• Average Interest Rate = AVERAGE(fact_loans[Interest_Rate])  
• NPA % = Non-Performing Loans / Total Loans  
```


## 3. Dashboard Highlights

### a. Overview
![Library_project](https://github.com/BijoyBytes/Power-Bi-Bank-Loan-Analysis/blob/main/Overview.png)


### b. Risk & Performance Analysis
![Library_project](https://github.com/BijoyBytes/Power-Bi-Bank-Loan-Analysis/blob/main/Risk.png)

## 📌 Recommendations

### 📉 Reduce Default Rate
* Identify high-risk loan types with elevated NPAs.
* Tighten credit checks for risky borrower segments.

### 💰 Improve Recovery Efficiency
* Prioritize recovery efforts in regions with low recovery rates.
* Introduce early repayment reminders and loan restructuring options.

### 📊 Optimize Loan Portfolio
* Increase focus on low-risk, high-return loan categories.
* Maintain a balanced mix of short-term and long-term loans.

### 🧑‍💼 Strengthen Credit Strategy
* Leverage borrower income, credit score, and repayment history for improved scoring.
* Limit approvals for consistently underperforming borrower segments.

### 📈 Drive Sustainable Growth
* Expand lending in regions with strong repayment performance.
* Apply risk-based interest rate adjustments to maximize returns.
