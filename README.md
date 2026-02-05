# 🚦 Traffic Collision Trends Analysis (2010–Present)

## 📌 Project Overview
This project analyzes historical traffic collision data from 2010 to the present to identify key patterns and risk factors related to **time, location, and victim demographics**.  
The goal is to convert raw accident data into actionable insights that can support **traffic management, public safety planning, and policy decisions**.

The project follows a structured Data Analytics lifecycle:
1. Problem Definition  
2. Data Cleaning & Preprocessing (Stage 2)  
3. Exploratory Data Analysis & Visualization (Stage 3)  
4. Documentation, Insights & Presentation (Stage 4)

---

## 🎯 Objectives
- Identify meaningful trends and patterns in traffic collisions over time  
- Detect high-risk time periods and geographic hotspots  
- Analyze demographic groups most affected by collisions  
- Create interactive visualizations and dashboards  
- Provide actionable recommendations for improving road safety  

---

## 🗂 Dataset Information
- **Source:** Government / Public Safety Open Data Portal  
- **Timeline:** 2010 – Present  
- **Records:** ~600,000+ rows  
- **Features:**  
  - DR Number  
  - Date Reported, Date Occurred, Time Occurred  
  - Area ID, Area Name, Reporting District  
  - Crime Code & Crime Code Description  
  - Victim Age, Victim Sex, Victim Descent  
  - Premise Description, Address, Location  
  - Derived fields: Year, Month, Month_Name, Weekday, Hour  

---

## 🛠 Tools & Technologies
- **Python:** pandas, numpy, matplotlib, seaborn  
- **Power BI:** Dashboard & KPI visualizations  
- **Jupyter Notebook / Google Colab:** Development environment  
- **Microsoft Word / PDF:** Final report documentation  

---

## 🔄 Project Workflow

### ✅ Stage 1 – Problem Definition & Initial Exploration
- Load dataset  
- Understand structure and data types  
- Perform basic EDA (shape, info, null checks, duplicates)

---

### ✅ Stage 2 – Data Cleaning & Preprocessing
- Handled missing values (median for numeric, mode for categorical)  
- Removed duplicate records  
- Converted date columns to datetime format  
- Treated outliers in Victim Age using IQR method  
- Created derived features:
  - Year  
  - Month  
  - Month Name  
  - Weekday  
  - Hour  

This ensured the dataset was clean, consistent, and analysis-ready.

---

### ✅ Stage 3 – Exploratory Data Analysis (EDA)
Visual analysis was performed to answer:

#### When do accidents happen?
- Accidents by Year  
- Accidents by Month  
- Accidents by Day of Week  
- Accidents by Hour of Day  

#### Where do accidents happen?
- Top 10 accident-prone areas  
- Area vs Year heatmap  
- Accident hotspot mapping  

#### Who is affected?
- Victim age distribution  
- Victim gender distribution  

#### What types of incidents occur?
- Crime Code Description  
- Premise Description  

Each visualization includes interpretation and business meaning.

---

### ✅ Stage 4 – Documentation & Insights
- Power BI dashboard with:
  - KPI Cards (Total Collisions, Peak Accident Hour, Most Dangerous Area, High Risk Day)  
  - Trend charts  
  - Maps and demographic analysis  
- Summary of findings in plain English  
- Key insights and business recommendations  
- Final executive summary and PDF report  

---

## 📊 Dashboard Features

### KPIs
- Total Collisions  
- Peak Accident Hour  
- Most Dangerous Area  
- High Risk Day  

### Visuals
- Line chart (Accidents by Year)  
- Bar charts (Hour, Weekday, Top Areas, Victim Age)  
- Pie chart (Victim Gender)  
- Heatmap (Area vs Year)  
- Map (Accident Hotspots)  

### Filters (Slicers)
- Year  
- Month  
- Area Name  

---

## 🔍 Key Insights
- Accidents peak between **4 PM and 7 PM** (rush hours)  
- **Friday** is the highest-risk day  
- A few areas (77th Street, Southwest, Wilshire, Olympic, Newton) are accident hotspots  
- Victims are mainly in the **20–50 age group**  
- Male victims account for about **60%** of collisions  
- Seasonal spikes occur in October, January, and August  

---

## 📌 Recommendations
- Increase traffic enforcement during peak hours  
- Improve infrastructure in hotspot areas  
- Run targeted safety campaigns for working-age adults  
- Strengthen Friday and weekend monitoring  
- Prepare additional resources during high-risk months

---

## 🏁 Conclusion

This project demonstrates how large-scale traffic collision data can be transformed into actionable insights using Python and Power BI.
The dashboard and analysis support evidence-based decision-making and provide a foundation for improving road safety strategies.

## 📁 Project Structure

```text
Traffic-Collision-Analysis/
│
├── data/
│   └── traffic_collision_cleaned.csv
│
├── notebooks/
│   └── Analysis_of_Traffic_Collision_Trends.ipynb
│
├── dashboard/
│   └── PowerBI_Dashboard.pbix
│
├── reports/
│   └── Stage4_Executive_Summary.pdf
│
└── README.md

