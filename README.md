# A-B-test-Campaign-performance-analysis
## Problem
Evaluate whether test campaign should be launched

## Approach
A/B testing + statistical validation

## Result
No significant improvement; test underperforms

## Decision
Do not roll out



##  Project Overview

This project evaluates the performance of two marketing campaigns (Control vs Test) using A/B testing principles to determine whether the new campaign should be rolled out.

The focus is not just on comparing metrics, but on **making a data-driven business decision** using statistical validation and behavioral analysis.

---

##  Business Problem

A new marketing campaign (Test) was introduced with the expectation of improving conversions.

The key question:
> **Should the test campaign be rolled out based on its performance?**

---

## Approach & Methodology

### 1️ Data Preparation & Cleaning
- Loaded and merged control and test datasets
- Handled delimiter inconsistencies and column formatting issues
- Standardized column names and data types
- Created a unified dataset for analysis

---

### 2️ Feature Engineering (Key Metrics)
Created business-relevant metrics:

- **Conversion Rate** = Purchases / Clicks  
- **Cost per Purchase** = Spend / Purchases  
- **Click-to-Purchase Rate**  
- **View-to-Cart Rate**

These metrics enabled performance comparison beyond raw counts.

---

### 3️ Exploratory Data Analysis (EDA)

- Compared control vs test performance across:
  - Conversion efficiency  
  - Cost efficiency  
  - Funnel behavior  

- Identified that:
  - Test campaign generated more traffic  
  - But had lower conversion efficiency  

---

### 4️ Statistical Testing

- Defined hypotheses:
  - **H0:** No difference in conversion rates  
  - **H1:** Significant difference exists  

- Used **Two-Sample T-Test** (daily aggregated data)

- Result:
  - p-value ≈ 0.139  
  - Not statistically significant  

---

### 5️  Funnel Analysis (Key Insight)

Analyzed user journey:

- Click → View → Add to Cart → Purchase  

 Major drop observed in:
> **View → Add to Cart stage (Test campaign)**

Indicates:
- Lower user intent or engagement  
- Possible issues with product experience or targeting  

---

##  Key Insights

- Conversion rate ↓ ~19% in test campaign  
- Cost per purchase ↑ ~17%  
- Traffic increased, but **quality decreased**  
- Funnel inefficiency identified in mid-stage  

---

##  Business Impact

- Prevented premature rollout of an underperforming campaign  
- Highlighted inefficiencies that could increase acquisition cost  
- Provided direction for targeted improvements in funnel stages  

---

##  Final Recommendation

> Do NOT roll out the test campaign.

Instead:
- Run further experiments with larger sample size  
- Investigate mid-funnel drop-offs  
- Improve targeting or user experience  

---

##  Dashboard

An interactive Power BI dashboard was created to:

- Compare campaign performance  
- Visualize funnel drop-offs  
- Present statistical results  
- Communicate final business decision  

---

##  Tools Used

- **Python (Pandas, NumPy)** → Data cleaning & analysis  
- **SciPy** → Statistical testing  
- **Power BI** → Visualization & dashboard  
- **Jupyter Notebook** → Workflow execution

---

##  Key Takeaways

- More traffic does not always mean better performance  
- Statistical significance is critical for decision-making  
- Funnel-level analysis provides deeper insights than top-level metrics  
- Business decisions should combine **data, statistics, and context**

---

##  Project Outcome

This project demonstrates the ability to:
- Perform end-to-end experimentation analysis  
- Apply statistical reasoning to real-world problems  
- Translate data into actionable business decisions  

---


