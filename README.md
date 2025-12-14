#💰 Loan Default Analysis Dashboard (Power BI)

## 📊 Project Overview

This project analyzes **loan portfolio performance, default risk, and borrower behavior** using **Power BI**. The dashboard helps financial institutions understand **loan distribution, risk factors, and performance trends** to support data‑driven lending decisions.

The solution is designed as a **3‑page interactive Power BI dashboard**:

1. **Loan Portfolio Summary**
2. **Risk Analysis Page**
3. **Loan Performance Page**

---

## 🧩 Problem Statement

Financial institutions need to monitor loan portfolios to:

* Identify **default risk drivers**
* Understand **borrower profiles**
* Track **loan performance across purposes and employment types**
* Improve **credit risk assessment and lending strategy**

This dashboard provides a clear view of **defaults, income, credit score, DTI ratio, interest rates, and loan purpose trends**.

---

## 🛠️ Tools & Technologies

* **Power BI Desktop**
* **Power BI Service**
* **CSV Dataset (Loan Default Data)**
* **DAX & Power Query**

---

## 🔄 Data Preparation Steps

### 1️⃣ Data Loading

* Loaded CSV dataset into **Power BI Desktop**

### 2️⃣ Data Profiling (Power Query)

* Enabled:

  * Column Distribution
  * Column Quality
  * Column Profile (Entire Dataset)

### 3️⃣ Data Cleaning

* Verified data types
* Handled missing values where applicable
* Ensured numeric columns (Income, Loan Amount, Credit Score, DTI Ratio, Interest Rate) were correctly formatted

---

## 📐 Dashboard Pages Explanation

---

## 📌 Page 1: Loan Portfolio Summary

### 🎯 Purpose

Provides a **high‑level snapshot** of the overall loan portfolio.

### 🔑 Key KPIs

* **Total Loans**
* **Total Loan Amount**
* **Average Credit Score**
* **Average Income**
* **Average Interest Rate**

### 📊 Visuals Used

* Gauge: Default Count vs Total Loans
* Bar Charts:

  * Loan Count by Education & Default Status
  * Loan Count by Employment Type & Default Status
* Column Chart: Total Loan Amount by Loan Purpose
* Bar Chart: Average Income by Employment Type

### 🎛️ Filters (Slicers)

* Loan Purpose
* Education
* Employment Type
* Loan Term

### 🔍 Insight

This page helps quickly identify **portfolio size, borrower strength, and default distribution** across key borrower attributes.

---

## 📌 Page 2: Risk Analysis Page

### 🎯 Purpose

Focuses on **credit risk indicators** and default behavior.

### 📊 Visuals Used

* Bar Chart: Defaults by Loan Purpose
* Pie Chart: Loan Amount Distribution by Default Status
* Line Chart: Average Income & Interest Rate Trend over Loan Date
* Scatter Plot:

  * Credit Score vs DTI Ratio by Default
* Table:

  * LoanID, Credit Score, DTI Ratio

### 🔍 Key Risk Indicators

* **Higher defaults linked with certain loan purposes**
* **Credit Score and DTI Ratio** show clear separation between default and non‑default loans
* Default loans contribute a **significant portion of total loan amount**

---

## 📌 Page 3: Loan Performance Page

### 🎯 Purpose

Analyzes **income, interest rate, and loan usage patterns**.

### 📊 Visuals Used

* Line Chart: Income vs Loan Amount
* Bar Chart: Average Interest Rate by Education
* Donut Chart: Income Distribution by Loan Purpose

### 🎛️ Filters (Slicers)

* Has Dependents
* Has Mortgage
* Education
* Loan Purpose
* Employment Type
* Marital Status
* Loan Term

### 🔍 Insight

This page highlights how **income and education impact interest rates and loan distribution**, helping evaluate borrower affordability.

---

## 🧮 Key DAX Measures

### 📌 Total Loans

```DAX
Total Loans = COUNT(LoanData[LoanID])
```

### 📌 Total Loan Amount

```DAX
Total Loan Amount = SUM(LoanData[LoanAmount])
```

### 📌 Average Credit Score

```DAX
Average Credit Score = AVERAGE(LoanData[CreditScore])
```

### 📌 Average Income

```DAX
Average Income = AVERAGE(LoanData[Income])
```

### 📌 Average Interest Rate

```DAX
Average Interest Rate = AVERAGE(LoanData[InterestRate])
```

---

## 📈 Key Insights

* Loan defaults are **not evenly distributed** across loan purposes
* Borrowers with **lower credit scores and higher DTI ratios** show higher default risk
* **Education level impacts interest rates** significantly
* Income patterns help assess **repayment capacity**
* Filters allow deep‑dive analysis for **risk‑based decision making**

---

## 🚀 Conclusion

This Power BI dashboard provides a **comprehensive loan risk and performance analysis**. It enables:

* Early identification of **default‑prone segments**
* Better **credit risk evaluation**
* Improved **lending and pricing strategies**

---

## 🖼️ Dashboard Screenshots

> *Below are snapshots of the Power BI dashboard pages included in this project.*

### 📌 Loan Portfolio Summary Page

* High-level KPIs (Total Loans, Loan Amount, Credit Score, Income, Interest Rate)
* Default count vs total loans
* Loan distribution by Education and Employment Type

📷 *Screenshot:*https://github.com/Surajkanekar3797/loan-default-analysis-powerbi/blob/main/1st%20Loan%20Portfolio%20summery.png

---

### 📌 Risk Analysis Page

* Default analysis by Loan Purpose
* Loan Amount distribution by Default status
* Credit Score vs DTI Ratio risk scatter
* Income & Interest Rate trend over time

📷 *Screenshot:*https://github.com/Surajkanekar3797/loan-default-analysis-powerbi/blob/main/2nd%20risk%20analysis%20Page.png

---

### 📌 Loan Performance Page

* Income vs Loan Amount trend
* Average Interest Rate by Education
* Income distribution by Loan Purpose
* Detailed slicers for borrower profiling

📷 *Screenshot:*https://github.com/Surajkanekar3797/loan-default-analysis-powerbi/blob/main/3d%20Loan%20Performance%20Page.png

---

## 📎 Project Type

* Data Analytics
* Financial Risk Analysis
* Power BI Dashboard

---

## 📬 Author
**Suraj kanekar**

If you have suggestions or feedback, feel free to connect.

⭐ *If you like this project, don’t forget to star the repository!*



