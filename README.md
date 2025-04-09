# 💼 Bank Marketing Campaign Analysis

This is an **unguided data analytics project** aimed at understanding the effectiveness of a bank's marketing campaign to promote term deposit subscriptions. Using **Power BI**, this project explores customer behavior and campaign performance to uncover patterns that can help in improving future marketing strategies.

---

## 📚 Table of Contents

- [Dataset Overview](#-dataset-overview)
- [Data Description](#-data-description)
- [Data Preparation & Cleaning](#-data-preparation--cleaning)
- [DAX Measures](#-dax-measures)
- [Visual Analysis Highlights](#-visual-analysis-highlights-power-bi)
- [Key Insights](#-key-insights)
- [Conclusion](#-conclusion)

---

## 📊 Dataset Overview

The dataset contains **45,000** customer records collected during a direct marketing campaign conducted by a Portuguese banking institution. The goal was to identify customers who are likely to subscribe to a **term deposit**.

### Summary Metrics:
- **Total Customers:** 45,000  
- **Total Subscriptions:** 5,000  
- **Subscription Rate:** 12%  
- **Average Call Duration:** 258 seconds  
- **Average Contacts per Campaign:** 3  

---

## 📋 Data Description

| Column Name                | Description                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| age                       | Age of the client                                                           |
| job                       | Job role of the client                                                      |
| marital                   | Marital status                                                              |
| education                 | Education level                                                             |
| default                   | Whether the client has credit in default                                    |
| balance                   | Account balance                                                             |
| housing                   | Whether the client has a housing loan                                       |
| loan                      | Whether the client has a personal loan                                      |
| contact                   | Contact communication type (e.g., cellular, telephone)                      |
| day                       | Last contact day of the month                                               |
| month                     | Last contact month                                                          |
| duration                  | Duration of the last contact (in seconds)                                   |
| campaign                  | Number of contacts during this campaign                                     |
| pdays                     | Days since the client was last contacted from a previous campaign           |
| previous                  | Number of contacts before this campaign                                     |
| poutcome                  | Outcome of the previous marketing campaign (renamed to `outcome`)           |
| y                         | Target variable (renamed to `term deposit subscribed`)                      |


---

## 🛠️ Data Preparation & Cleaning

The dataset was preprocessed and enhanced with additional features for more insightful visualizations:

- ✅ Added new columns:
  - `age group`
  - `balance range`
  - `duration group`
  - `sr. no`
- ✅ Renamed columns for clarity:
  - `poutcome` ➝ `outcome`
  - `y` ➝ `term deposit subscribed`
- ✅ Ensured consistency in data types, handled missing values, and prepared the data for Power BI analysis.

---

## 📐 DAX Measures

To support KPI tracking and visual analysis, the following custom measures were created in Power BI:

- **Subscription Rate:** Percentage of customers who subscribed to a term deposit  
- **Conversion Rate:** Percentage of successful subscriptions among customers who were actually contacted

These measures were used across visuals like stacked bar charts, combo charts, and KPI cards to highlight key performance indicators.

---

## 📈 Visual Analysis Highlights (Power BI)

### 📊 Subscription Rate by Age Group
- **Highest:** Age 70+ (45.08%)  
- **Lowest:** Age 31–50 (9.79%)

### 💼 Subscription Outcome by Job Role
- **Best performers:** Students (29%), Retired (23%)  
- **Lowest:** Blue-collar (7%)

### 💰 Balance Range vs Conversion Rate
- Highest conversions in **1001–2000** balance range (17%)  
- Majority of customers have balance under **1000**

### 📞 Previous Campaign Outcome vs Subscription Rate
- Customers with previous success: **64.77%** conversion rate  
- "Unknown" outcomes: only **9.16%**

### ⏱️ Call Duration vs Conversion
- Longer calls result in significantly higher conversion rates

---

## 💡 Key Insights

- Focus future campaigns on **retired individuals**, **students**, and those aged **70 and above**
- Clients with **successful prior engagements** are much more likely to subscribe
- Conversion improves significantly with **longer conversations**
- Moderate **account balance** correlates with higher subscription likelihood

---

## ✅ Conclusion

This project provides a comprehensive understanding of which customer segments are most likely to respond positively to term deposit campaigns. The use of Power BI helped uncover patterns and trends through clear, interactive visualizations that can guide strategic marketing decisions in future campaigns.
