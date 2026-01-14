# Healthcare-Analysis-Dashboard

🏥 Healthcare Waiting List Analytics – Power BI Dashboard
📌 Project Summary

This project delivers an enterprise-grade Power BI analytics solution for monitoring and analyzing healthcare patient waiting lists. The dashboard is built using publicly available inpatient and outpatient data (2018–2021) and follows a full BI development lifecycle, from business requirement gathering to deployment and maintenance.

The solution enables healthcare decision-makers to track waiting list volumes, identify trends, compare year-over-year performance, and analyze demand across specialties and age groups through an interactive and scalable reporting layer.

🎯 Business Problem

Healthcare providers require timely visibility into patient waiting lists to:

Monitor service pressure across specialties

Identify long-term waiting patterns

Compare current demand against historical benchmarks

Support operational planning and capacity management

Raw Excel-based reporting lacks scalability, consistency, and interactivity. This dashboard addresses those gaps using a centralized Power BI model.

🛠 Technology Stack

Power BI Desktop

Power Query (M Language)

DAX

Excel (Source Data)

Power BI Service (Publishing & Sharing)

📂 Data Overview

Source: Public healthcare waiting list dataset

Coverage: 2018–2021

Data Domains:

Inpatient

Day Case

Outpatient

Key Dimensions:

Specialty

Case Type

Age Profile

Time Band

Date (Monthly granularity)

🧠 BI Development Approach
1. Requirements & Stakeholder Alignment

Defined reporting objectives with a focus on operational KPIs

Identified core metrics:

Total waiting list

Average waiting list

Median waiting list

Established reporting scope:

Executive summary view

Detailed analytical view

Documented assumptions and data limitations

2. Data Ingestion

Implemented folder-based ingestion to support scalable file updates

Validated schema consistency across all source files

Combined inpatient and outpatient datasets during load

3. Data Transformation & Modeling

Standardized column naming and data types

Resolved data quality issues (missing values, inconsistent labels)

Created a unified fact table for reporting

Added a specialty mapping dimension to support grouped analysis

Built and validated relationships in Model View

Hid staging tables to simplify report consumption

4. Semantic Model & DAX

Developed reusable DAX measures for:

Latest available month logic

Year-over-year comparison

Average vs median calculations

Implemented metric toggle functionality using slicers

Ensured measures return zero instead of blanks where required

5. Report & Dashboard Design

Summary Page

KPI cards (current vs same month previous year)

Case type distribution (donut chart)

Age profile vs time band analysis

Top 5 specialties by selected metric

Monthly trend analysis by care type

Global slicers for time, specialty, and case type

Detail Page

Advanced matrix for granular exploration

Context-aware filtering

Page navigation controls

Design principles applied:

Grid-based alignment

Consistent color palette

Dynamic titles and labels

Minimal visual clutter

6. Interactivity & User Experience

Controlled slicer interactions per visual

Implemented tooltip pages for deeper insights

Added user feedback messaging for empty states

Enabled intuitive page navigation with hover tooltips

7. Testing & Validation

Functional testing of all slicers and visuals

Validation of DAX calculations

Cross-checking totals against source data

UX testing for navigation and usability

🏁 Conclusion

This project demonstrates a production-ready Power BI solution built using industry best practices in data modeling, DAX, and dashboard design. The approach is transferable across healthcare and other data-intensive domains requiring operational analytics.
