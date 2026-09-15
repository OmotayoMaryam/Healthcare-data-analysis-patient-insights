# Healthcare Data Analysis & Patient insights Dashboard
Healthcare data analysis and patient insights dashboard built with Power BI, Power Query, and DAX

# Project Overview
Healthcare organizations generate large volumes of patient, visit, diagnosis, treatment, provider, and operational data. When properly analyzed, this data can provide valuable insights into patient behavior, healthcare utilization, service delivery, satisfaction, and operational performance.

For this project, I analyzed a healthcare dataset and developed an interactive Power BI dashboard to transform raw healthcare records into meaningful insights that can support data-driven decision-making.

The project focuses on understanding:
* Patient demographic
* Healthcare Utilization
* Department Performance
* Diagnosis Patterns
* Patient Satisfaction
* Service type Utilization
* Repeat patient behavior
* Healthcare costs

The objective was not to only visualize the data, but to use the data to answer practical healthcare business questions and identify patterns that could support better resource allocation and patient service delivery.

# Business Problem
Healthcare organizations need to understand how patients interact with their services and how resources are being utilized across departments.

Without an effective reporting system, important questions can be difficult to answer:
* Which departments receive the highest number of visits?
* Which diagnoses account for the greatest number of visits?
* Are patients distributed evenly across genders?
* Which age groups are most affected by specific diagnoses?
* Which service types have the highest patient satisfaction?
* How many patients are returning for additional visits?
* How does patient satisfaction vary across departments?
* What patterns exist in patient satisfaction scores?
* How are healthcare services distributed across locations?
* Where are potential opportunities for operational improvement?

This Project addresses these questions by converting healthcare records into an interactive analytical dashboard

# Data Structure
This dataset is organized into multiple related tables.

| Table | Purpose |
|-------|---------|
| Patients | Contains patient-level information |
| Visits | Contains healthcare visit/encounter information |
| Departments | Contains healthcare department information |
| Diagnoses | Contains diagnosis-related information |
| Procedures | Contains procedure information |
| Providers | Contains healthcare provider information |
| Insurance | Contains insurance-related information |
| Cities | Contains geographic/location information |
| DateTable | Supports date-based analysis |

These tables were loaded into Power BI and used to build the analytical model

# Tools Used
Power BI
Used for:
* Data modelling
* Data tranformation
* Data visualization
* KPI development
* DAX calculations
* Interactive dashboard development
* Slicers and filtering
* Business intelligence storytelling

Power Query
 Power Query was used during the data preparation stage to inspect and transform the source data.

One of the data-quality issues identified involved the Follow-Up Visit Date field. The field contained valid dates alongside null values and errors, requiring transformation and validation before it could be reliably used for analysis.

DAX
DAX measures were used to create analytical KPIs and calculated metrics for the dashboard.

Examples include:

* Patient counts
* Visit counts
* Repeat patient metrics
* Average satisfaction
* Percentage calculations
* Rate-based KPIs

# Data Preparation Process
The project followed a structured analytics workflow:
Raw Healthcare Data → Data Cleaning → Data Modelling → DAX Measures → Visualization → Analysis → Insights

1. Data Inspection

The source data was first inspected to understand:

* Available tables
* Column names
* Data types
* Relationships
* Missing values
* Errors
* Duplicate or inconsistent records

The healthcare model contains multiple tables, including patients, visits, diagnoses, departments, providers and procedures.

2. Data Cleaning
Power Query was used to identify and address data-quality issues.

Particular attention was given to date fields because some records contained:

* Valid dates
* Null values
* Errors

For example, the Follow-Up Visit Date field showed valid records alongside null and error values.
Cleaning these issues was important because inaccurate date fields could affect:

* Follow-up analysis
* Time-based reporting
* Patient retention analysis
* Visit trends

3. Data Modelling
The dataset was structured into multiple related tables.

This approach makes it possible to analyze healthcare activity from different perspectives while reducing unnecessary duplication of information.

A dedicated DateTable was also included to support time-based analysis.

# Dashboard Structure
The Power BI report was designed across multiple pages.

Page 1: Overview

The Overview page provides a high-level summary of healthcare activity.

The purpose of this page is to give users a quick understanding of the overall state of the healthcare operation before drilling into specific areas.

Potential areas covered include:

* Patient volume
* Visit activity
* Satisfaction
* Healthcare utilization
* Overall performance

Page 2: Department & Patient Analysis

This page focuses on the relationship between patients, departments, diagnoses and healthcare services.

The dashboard contains KPIs and visuals including:

* Repeat Patients
* Emergency Visit Rate
* Average Satisfaction
* Total Visits by Department
* Total Patients by Gender
* Total Visits by Diagnosis
* Diagnosis by Age Group
* Average Satisfaction by Department
* Total Visits by Insurance provider

Page 3: Cost Analysis 

The Cost Analysis page focuses on understanding healthcare spending and identifying patterns in treatment-related costs.

The analysis can help answer questions such as:

* Which departments generate the highest healthcare costs?
* Which diagnoses are associated with higher treatment costs?
* How do costs vary across patient groups?
* Which procedures contribute most to overall healthcare expenditure?

This provides a financial perspective that can support cost control, resource allocation, and operational planning.

# Key Findings
* Cardiology recorded the highest number of visits among the departments analyzed, with 1,281 visits.
* Hypertension was the most frequent diagnosis, accounting for 2,013 visits.
* The patient population was almost evenly split by gender, with 50.05% female and 49.95% male.
* Average patient satisfaction was approximately 4 out of 5.
* Inpatient and emergency services recorded higher average satisfaction than outpatient services.
* The dataset contained data-quality issues, including invalid and missing Follow-Up Visit Date values, which required cleaning before analysis.

# Business Recommendations

Based on the analysis, healthcare providers can:

* Monitor high-volume departments to ensure adequate staffing and resources.
* Investigate the high prevalence of hypertension and strengthen preventive-care initiatives.
* Improve outpatient service delivery to address comparatively lower satisfaction.
* Monitor healthcare costs by department, diagnosis, and procedure.
* Improve data-quality processes to ensure more reliable reporting and decision-making.

# Conclusion

This project demonstrates how healthcare data can be transformed into actionable insights using Power BI. From data cleaning and modelling to KPI development, visualization, and recommendations, the dashboard provides a structured view of patient activity, healthcare services, satisfaction, and costs.
