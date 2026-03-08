
# 🏥 NHS England Emergency Readmissions Dashboard

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-F2C811?logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-Visualization-blue?logo=python)
![DAX](https://img.shields.io/badge/Language-DAX-purple)
![Status](https://img.shields.io/badge/Project-Portfolio%20Project-success)

## 📊 Project Overview
This project presents a comprehensive **Power BI dashboard** analyzing emergency hospital readmissions across England.

The analysis uses the **NHS England I02040 Compendium Emergency Readmissions dataset**, which tracks the rate at which patients are readmitted to hospital **within 30 days of discharge**.

Emergency readmissions are a key healthcare performance indicator because high rates may signal:
- Poor discharge planning
- Limited community healthcare support
- Ineffective follow‑up care after hospital treatment

The dashboard provides interactive insights into **national trends, regional variation, provider performance, and socioeconomic inequality** in readmission outcomes.

---

# 🗂 Dataset Summary

| Field | Description |
|------|-------------| Dataset | NHS England I02040 Compendium |
| Coverage | 2014/15 – 2024/25 |
| Records | 155,573 |
| Geographic Scope | England |
| Data Levels | National, Regional, Provider, Deprivation Groups |
| Metric | Emergency Readmission within 30 Days |

---

# 🧹 Data Preparation

Data preparation and transformation were performed in **Power Query**.

Key steps:

• Removed 15‑row title block from the raw dataset  
• Promoted proper column headers  
• Corrected numeric data types  
• Cleaned and structured categorical fields  
• Prepared columns for Power BI modelling

Important fields include:

- Indicator Value
- Numerator
- Denominator
- Year
- Region
- Sex
- Age Group
- Deprivation Quintile

---

# 📐 Data Modeling & DAX

A full set of **DAX measures** was developed to power the dashboard's KPIs and analytics.

Examples include:

- National Readmission Rate
- Year‑over‑Year Change
- Provider Performance Counts
- Deprivation Inequality Gap
- Dynamic KPI Cards
- Conditional Performance Banding

These calculations allow all visuals to **update dynamically based on slicer selections**.

---

# 📊 Dashboard Features

The report is designed as a **multi‑page interactive Power BI dashboard** with a global slicer panel.

### Global Filters
- Financial Year
- Sex
- Age Group
- Breakdown Category

### Core Visualizations

**KPI Cards**
- National Readmission Rate
- Total Readmissions
- Deprivation Gap
- Provider Performance

**Trend Analysis**
- National readmission trend (2014–2024)

**Regional Performance**
- Horizontal bar chart comparing regional rates

**Provider Performance Distribution**
- Donut chart showing provider banding

**Socioeconomic Analysis**
- Readmission rate by deprivation quintile
- Deprivation trend over time

**Year‑over‑Year Analysis**
- Annual change in readmission rates

---

# 🐍 Advanced Visualization

A **Python visual using Matplotlib** was embedded within Power BI to generate a custom donut chart.

Benefits:
- Custom center text labels
- Advanced styling
- Publication‑quality visual output
- Dynamic updates based on dashboard filters

This demonstrates how **Python scripting can extend Power BI’s native visualization capabilities**.

---

# 📈 Key Insights

## 1️⃣ Long‑Term Rise in Readmissions
England's emergency readmission rate increased from:

**12.6% (2014/15) → 14.8% (2023/24)**

This represents a **17% relative increase** over a decade.

---

## 2️⃣ COVID‑19 Caused the Largest Spike
The **2020/21 financial year** saw the largest single increase:

**+1.10 percentage points**

This spike reflects disruptions in hospital operations during the pandemic.

---

## 3️⃣ National Performance Snapshot (2023/24)

| Metric | Value |
|------|------|
| Total Readmissions | 939,000 |
| Eligible Admissions | 6.34 Million |
| National Rate | 14.8% |

Provider distribution:

- 47% Better than expected
- 37% Within expected range
- 15% Alert (> expected)

Approximately **1 in 6 hospitals require further investigation**.

---

## 4️⃣ Regional Variation

Highest rate:
**South West – 15.8%**

Lowest rate:
**East of England – 13.8%**

Regional performance varies by **~2 percentage points**, indicating differences in healthcare capacity and population needs.

---

## 5️⃣ Socioeconomic Inequality

Emergency readmissions show a strong deprivation gradient.

| Deprivation Group | Readmission Rate |
|------------------|-----------------|
| Most Deprived | 15.0% |
| Least Deprived | 13.1% |

This represents a **1.9 percentage point inequality gap** that has remained consistent over time.

---

# 🧠 Conclusion

The analysis highlights three major systemic patterns:

• Readmission rates are **rising nationally**  
• **Regional disparities** remain significant  
• **Socioeconomic deprivation strongly impacts outcomes**

Reducing emergency readmissions will require:

- Improved discharge planning
- Expanded community healthcare support
- Targeted intervention in high‑risk regions and populations

---

# ⚙️ Technology Stack

| Tool | Purpose |
|----|----|
Power BI | Dashboard development |
Power Query | Data cleaning & transformation |
DAX | Data modeling and KPI calculations |
Python (Matplotlib) | Custom visualization |
Excel | Raw data source |

---

# 📷 Dashboard Preview

```
NHS_Readmission_Report.pdf
```

---

# 🚀 How to Use

1️⃣ Download the `.pbix` file from the repository  
2️⃣ Open using **Power BI Desktop**  
3️⃣ Explore the dashboard using slicers and filters  
4️⃣ Analyze national, regional, and socioeconomic trends



---

# 📌 Future Improvements

• Forecasting model for future readmission trends  
• Hospital‑level drill‑through analysis  
• Integration with live NHS datasets  
• Additional demographic segmentation  

---

# 👨‍💻 Author

Ajay Kumar
Data Analytics Portfolio Project  
Built to demonstrate **Power BI, DAX, Python visualization, and healthcare analytics skills**.
