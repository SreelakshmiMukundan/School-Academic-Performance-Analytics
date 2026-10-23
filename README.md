# School-Academic-Performance-Analytics
School academic performance and attendance analysis using Excel, Power Query and Power BI, featuring an interactive executive dashboard.
# School Academic Performance & Attendance Analytics

**An interactive school analytics project built using Excel, Power Query, Power BI and DAX.**

This project explores student examination performance, attendance, study habits, academic support, wellbeing and family background. It transforms a synthetic Kaggle dataset into an executive dashboard and five detailed report pages to help school administrators explore academic patterns and identify areas for further investigation.

> **Data note:** The dataset is synthetic and does not represent any real school or student. Findings are descriptive associations, not evidence of causation.

## Project Overview

| Item | Details |
|---|---|
| Dataset | [Student Performance Factors – Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors) |
| Records | 6,607 |
| Original columns | 20 |
| Tools | Excel, Power Query, Power BI Desktop, DAX |
| Deliverables | 1 executive dashboard + 5 detailed analysis pages |

## Objectives

- Explore examination score distributions and identify lower-scoring groups using project-defined performance bands.
- Examine relationships between attendance, study hours, previous scores and current performance.
- Compare academic patterns across tutoring, school environment, learning resources and student wellbeing.
- Explore parental involvement, education, family income and demographic distributions.
- Present findings through interactive visuals to support management-level analysis.

## Data Cleaning & Transformation

Data profiling and preparation were performed using Excel and Power Query.

- Checked data quality, data types and duplicate records; no exact duplicate rows were identified.
- Identified 235 missing cells across three categorical fields and replaced missing values with `Not Recorded`.
- Applied Trim and Clean operations to standardise categorical text.
- Created a technical `Record_ID` for record-level analysis.
- Added calculated columns for exam performance bands and grouped fields for study hours, attendance and previous scores.
- Investigated an exam score of 101 and applied an assumed maximum of 100 in the cleaned data, retaining the original source separately.

**Performance bands:** Needs Support (below 65), Developing (65–74), Proficient (75–84) and High Achievement (85 or above). These are analyst-defined thresholds, not official school assessment standards.

## Power BI Dashboard & DAX

Developed an interactive report with KPI cards, charts, matrices, scatter plots and slicers for Gender and School Type.

Key measures include:

- Total Records
- Average Exam Score
- Average Previous Score
- Average Attendance
- Lower Score Share
- Average Study Hours
- Highest Exam Score
- Average Sleep Hours and Physical Activity

## Report Pages

| Page | Analysis Focus |
|---|---|
| Executive Dashboard | Overall KPIs, performance bands, attendance, study hours and parental involvement |
| 1. Academic Performance Overview | Score distribution, performance categories and previous attainment |
| 2. School Environment & Support | Attendance, tutoring, teacher quality, peer influence and school type |
| 3. Study Habits & Learning Resources | Study time, learning resources, internet access and previous scores |
| 4. Student Wellbeing & Engagement | Sleep, motivation, physical activity and extracurricular participation |
| 5. Family Background & Demographics | Parental involvement, education, income, home distance and gender distribution |

## Key Findings

- **Average exam score:** 67.24/100.
- **Average attendance:** 79.98%.
- **Below-65 score share:** 21.98% of records.
- **Performance distribution:** 76.15% of records fell into the Developing band, based on the project's defined score ranges.
- **Attendance and study habits:** Higher attendance and study hours showed positive descriptive associations with average exam scores.
- **Tutoring and parental involvement:** Average scores generally increased across tutoring-session categories and parental involvement levels.
- **Family background:** The average score was 68.60 for the Postgraduate/High Income group and 66.50 for the High School/Low Income group.

These findings describe patterns in the synthetic dataset and do not prove that any factor causes improved or reduced performance.

## Potential Management Applications

With validated real-school data, similar analysis could help administrators:

- Identify academic areas that may need additional review or support.
- Investigate attendance patterns and potential barriers.
- Evaluate tutoring and learning-support initiatives.
- Explore student engagement, wellbeing and family-support patterns.
- Monitor KPIs through interactive reports and filtered comparisons.

## Project Files

- **Power BI report (`.pbix`):** Interactive executive dashboard and five detailed report pages.
- **Project documentation (`.docx`):** Data dictionary, cleaning decisions, calculated fields, DAX measures, findings and recommendations.
- **Dashboard screenshots (`.png`):** Visual previews, where available.

Open the `.pbix` file in Power BI Desktop to explore the report and its interactive slicers.

## Limitations & Responsible Use

- The dataset is synthetic and cross-sectional; it does not contain real student identities or longitudinal school records.
- The performance bands and 100-point score cap are project assumptions.
- Observed relationships are not causal evidence.
- Sensitive factors such as gender, family income and learning-disability status should not be used to make automated high-stakes decisions about individual students.

**Skills demonstrated:** Data profiling, data cleaning, Power Query transformations, data validation, calculated columns, DAX measures, KPI development, exploratory data analysis, interactive dashboard design and data storytelling.
## Executive Dashboard

![School Academic Performance Executive Dashboard](screenshots/executive-dashboard.png)
