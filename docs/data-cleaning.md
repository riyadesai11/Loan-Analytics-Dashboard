# Data Cleaning Notes

## Overview
The raw loan dataset was cleaned in **Power Query / Power BI** before building the dashboard.  
The goal was to make the data suitable for **portfolio analysis, borrower risk analysis, and debt / credit exposure analysis**.

---

## Main Cleaning Steps

### 1. Credit Score
- Cleaned missing / inconsistent values
- Retained final usable credit score field for analysis
- Used for **Avg Credit Score**, **Risk Band**, and borrower risk visuals

### 2. Years in Current Job
- Standardized values like `10+ years`, `2 years`, etc.
- Cleaned for use in slicers and borrower segmentation

### 3. Current Loan Amount
- Handled missing values
- Kept as core field for **Total Loan Amount** and **Avg Loan Amount**

### 4. Annual Income
- Cleaned missing values
- Used for **Avg Annual Income**, **Income Band**, and debt analysis

### 5. Monthly Debt
- Retained as numeric field for debt burden analysis

### 6. Delinquency Field
- Used **Months since last delinquent** to create **Delinquency Flag**

### 7. Bankruptcies
- Converted into **Bankruptcy Flag

### 8. Tax Liens
- Converted into **Tax Lien Flag

---

## Derived Fields Created
- **Income Band**
- **Risk Band**
- **Delinquency Flag**
- **Bankruptcy Flag**
- **Tax Lien Flag**
- **Credit Utilization logic support**

---

## Main Columns Used in Dashboard
- Current Loan Amount
- Term
- Credit Score
- Annual Income
- Years in current job
- Home Ownership
- Purpose
- Monthly Debt
- Months since last delinquent
- Current Credit Balance
- Maximum Open Credit
- Bankruptcies
- Tax Liens

---

## Low-Value / Technical Columns
- Loan ID
- Customer ID

These were mainly used for counting or record identification, not for direct insight visuals.
