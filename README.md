.# School-Academic-Performance-Analytics

School academic performance and attendance analysis using Excel, Power Query and Power BI, featuring an interactive executive dashboard.

# School Academic Performance & Attendance Analytics

**An interactive school analytics project built using Excel, Power Query, Power BI and DAX.**

This project explores student examination performance, attendance, study habits, academic support, wellbeing and family background. It uses a Kaggle dataset to develop an executive dashboard and five detailed analytical report pages, helping school administrators explore academic patterns and identify areas for further investigation.

## Project Overview

| Item | Details |
|---|---|
| Dataset | [Student Performance Factors – Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors) |
| Records | 6,607 |
| Original columns | 20 |
| Data preparation | Microsoft Excel and Excel Power Query |
| Visual analytics | Power BI Desktop, Power Query and DAX |
| Deliverables | 1 executive dashboard and 5 detailed analytical report pages |

## Objectives

- Explore examination score distributions and identify lower-scoring groups using project-defined performance bands.
- Examine relationships between attendance, study hours, previous scores and current examination performance.
- Compare academic patterns across tutoring, school environment, learning resources and student wellbeing.
- Explore parental involvement, parental education, family income, home distance and demographic distributions.
- Present findings through interactive visualizations to support management-level analysis and decision-making.

## Data Understanding

The dataset contains 6,607 records and 20 original fields, comprising 7 numerical fields, 8 ordinal categorical fields and 5 nominal categorical fields.

Initial data profiling identified 235 missing cells across three categorical fields.

| Field | Missing cells | Treatment |
|---|---:|---|
| Teacher_Quality | 78 | Replaced with `Not Recorded` |
| Parental_Education_Level | 90 | Replaced with `Not Recorded` |
| Distance_From_Home | 67 | Replaced with `Not Recorded` |
| **Total** | **235** | |

## Data Cleaning & Transformation

Data profiling, preparation and validation were performed using Excel and Power Query.

- Checked data quality, data types and duplicate records; no exact duplicate rows were identified during source profiling.
- Replaced 235 missing categorical values across three fields with `Not Recorded`.
- Applied Trim and Clean operations to standardize categorical text.
- Validated numerical and categorical data types.
- Created a technical `Record_ID` using a Power Query index. This identifies records and is not an actual student ID.
- Created `Exam_performance_bands` to group examination scores.
- Grouped study hours, attendance and previous scores into ranges for comparative analysis.
- Investigated an original examination score of 101 against an assumed maximum of 100. The original source data was retained unchanged, and the score boundary was documented as a validation limitation.

### Project-Defined Performance Bands

| Performance band | Exam score |
|---|---|
| Needs Support | Below 65 |
| Developing | 65–74 |
| Proficient | 75–84 |
| High Achievement | 85 and above |

These thresholds were defined for this project. They are not official school grading or pass/fail standards.

## Power BI Dashboard & DAX

Developed an interactive Power BI report with KPI cards, charts, matrices, scatter plots and slicers for Gender and School Type.

### Key Performance Indicators

- Total Records
- Average Exam Score
- Average Previous Score
- Highest Exam Score
- Average Attendance
- Students Scoring Below 65
- Average Study Hours
- Average Sleep Hours
- Average Physical Activity

The report supports interactive filtering, allowing users to compare academic patterns across available categories.

## Report Pages

| Page | Analysis focus |
|---|---|
| Executive Dashboard | Overall KPIs, performance bands, attendance, study hours and parental involvement |
| 1. Academic Performance Overview | Score distribution, performance categories and previous attainment |
| 2. School Environment & Support | Attendance, tutoring, teacher quality, peer influence and school type |
| 3. Study Habits & Learning Resources | Study time, learning resources, internet access and previous scores |
| 4. Student Wellbeing & Engagement | Sleep, motivation, physical activity and extracurricular participation |
| 5. Family Background & Demographics | Parental involvement, education, income, home distance and gender distribution |

## Key Findings

### Overall Performance

- **Total records:** 6,607.
- **Average exam score:** 67.24 out of 100.
- **Average previous score:** 75.07 out of 100.
- **Average attendance:** 79.98%.
- **Records scoring below 65:** 1,452 (21.98%).
- **Average study hours:** 19.98.
- **Highest cleaned exam score:** 100.

### Performance Distribution

| Performance band | Records | Percentage |
|---|---:|---:|
| Needs Support | 1,452 | 21.98% |
| Developing | 5,031 | 76.15% |
| Proficient | 89 | 1.35% |
| High Achievement | 35 | 0.53% |

Percentages may differ slightly from 100% due to rounding.

### Additional Insights

- **Attendance:** Higher attendance levels were generally associated with higher average examination scores.
- **Study habits:** Students with more study hours generally showed higher average examination scores.
- **Tutoring:** Average scores generally increased across tutoring-session categories. This does not establish that tutoring caused the differences.
- **School environment:** Average scores across Public and Private school categories were both around 67, with only small differences.
- **Parental involvement:** Average scores increased slightly across Low, Medium and High parental-involvement categories.
- **Family background:** The Postgraduate / High Income group had an average score of 68.60, compared with 66.50 for the High School / Low Income group.
- **Wellbeing and engagement:** The report explores sleep, motivation, physical activity and extracurricular participation in relation to examination performance.
- **Extracurricular participation:** Among students without reported learning disabilities, average scores were 67.55 for those participating in extracurricular activities and 67.05 for those not participating. Among students with reported learning disabilities, the corresponding averages were 66.47 and 65.99.

These findings describe patterns and associations in the selected dataset. They do not establish cause and effect.

## Potential Management Applications

With appropriate validation and authorized school data, similar analytical approaches could help administrators:

- Identify academic areas that may need additional review or support.
- Explore attendance patterns and potential barriers to regular attendance.
- Review tutoring and learning-support initiatives.
- Explore student engagement, wellbeing and family-support patterns.
- Monitor KPIs through interactive dashboards and filtered comparisons.

These are potential applications rather than outcomes validated through deployment in a specific school.

## Project Files

- **Power BI report (`.pbix`):** Interactive executive dashboard and five detailed analytical report pages.
- **Excel workbook (`.xlsx`):** Original data and prepared data, as included in the workbook.
- **CSV dataset (`.csv`):** Dataset file for analysis.
- **Project documentation (`.docx`):** Data dictionary, cleaning decisions, calculated fields, DAX measures, findings, recommendations and limitations.
- **Dashboard image (`.png`):** Static preview of the executive dashboard.

Open the `.pbix` file in Power BI Desktop to explore the report and its interactive slicers.

## Limitations, Ethics & Validation Priorities

- **Dataset scope:** The selected Kaggle dataset may not reflect the circumstances of a specific school or actual UAE educational outcomes.
- **Cross-sectional data:** The dataset does not contain dates or actual student IDs, so changes over time and longitudinal student outcomes cannot be analysed.
- **Non-causal analysis:** Observed relationships may reflect other factors and do not establish cause and effect.
- **Score assumptions:** The original data contains an examination score of 101. An assumed maximum of 100 requires validation against the original score definition. The original source data was retained unchanged.
- **Performance bands:** The score categories are analyst-defined and are not official school assessment standards.
- **Missing data:** Missing categorical entries were labelled `Not Recorded`. These missing values may affect group comparisons.
- **Fairness and privacy:** Gender, family income, learning-disability status and other student characteristics should be handled responsibly and should not be used alone to make high-stakes decisions about individuals.
- **Further validation:** Group sizes, score definitions, transformations, DAX measures and filters should be checked before applying similar analysis to real educational decisions.

## Skills Demonstrated

Data profiling, data cleaning, Excel, Power Query transformations, data validation, calculated columns, DAX measures, KPI development, exploratory data analysis, interactive dashboard design, data interpretation, management reporting and data storytelling.

## Executive Dashboard

![School Academic Performance Executive Dashboard](screenshots/executive-dashboard.png)

## Author

**Sreelakshmi K M**

Data Analytics | Power BI | Excel | SQL | Python

[LinkedIn](https://www.linkedin.com/in/sreelakshmimukundan/) · [GitHub](https://github.com/SreelakshmiMukundan)

---

### Repository Topics

`data-analytics` `power-bi` `excel` `power-query` `dax` `dashboard` `data-visualization` `student-performance` `education-analytics` `business-intelligence` `data-cleaning` `kaggle`

## Executive Dashboard

![School Academic Performance Executive Dashboard](screenshots/executive-dashboard.png)
