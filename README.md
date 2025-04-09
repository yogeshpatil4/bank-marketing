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
| age group (new)           | Age categorized into bins                                                   |
| balance range (new)       | Balance categorized into ranges                                             |
| duration group (new)      | Duration categorized into groups                                            |
| sr. no (new)              | Serial number added for easy reference                                      |

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
- ✅ Ensured consistency in data types, handled missing values, and prepared the data for
