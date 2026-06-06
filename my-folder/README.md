# Healthcare Performance Analytics Dashboard

![Dashboard Preview](screenshots/01_executive_summary.png)

## Project Overview
An end-to-end Power BI dashboard analyzing 10,252 patient records 
to uncover insights across clinical outcomes, doctor performance, 
and financial operations.

**Tools Used:** Power BI Desktop, DAX, Power Query  
**Dataset:** Synthetic Healthcare Dataset (Kaggle)  
**Pages:** 5 | **Records Analyzed:** 10,252

---

## Dashboard Pages
| Page | Business Question |
|------|------------------|
| Executive Summary | Is the hospital performing well overall? |
| Patient Demographics | Who are our patients? |
| Clinical Insights | Where are clinical outcomes failing? |
| Doctors Performance | Which doctors drive the most value? |
| Finance & Operations | Where is revenue concentrated? |

---

## Key Insights
- 57% of patients received abnormal test results, 
  with Asthma showing the highest rate at 56%
- Tuberculosis has the highest readmission rate at 15.07% 
  vs Asthma at 11.02% — a 37% relative gap
- Emergency admissions generate 2x total revenue ($105M) 
  vs Elective ($55M)
- Cancer is the highest cost condition at $30.9K avg billing — 
  36% higher than Asthma
- Top doctor (Randy Scott) generates $22.44M vs lowest performer 
  at $2.03M — an 11x revenue gap
- June and October identified as peak admission months 
  for proactive staffing

---

## Dashboard Screenshots

### Executive Summary
![Executive Summary](screenshots/01_executive_summary.png)

### Patient Demographics
![Patient Demographics](screenshots/02_patient_demographics.png)

### Clinical Insights
![Clinical Insights](screenshots/03_clinical_insights.png)

### Doctors Performance
![Doctors Performance](screenshots/04_doctors_performance.png)

### Finance & Operations
![Finance Operations](screenshots/05_finance_operations.png)

---

## Technical Details

**Data Model:** Star schema with fact and dimension tables  
**DAX Measures Written:**
- Readmission Rate %
- Abnormal Test Rate %
- Avg Billing Amount
- Total Revenue
- Avg Patient Rating
- Avg Patients per Doctor

**Power Query Steps:**
- Data type correction
- Index column added as Patient ID surrogate key
- Age group calculated column
- Null handling on critical columns

---

## How to View
1. Download `Healthcare_Dashboard.pbix`
2. Open in Power BI Desktop (free download from Microsoft)
3. Use Medical Condition and Year slicers to filter all pages

---

*Dataset is synthetic and used for portfolio demonstration purposes only.*
