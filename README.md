Emergency Room Performance Dashboard

A complete end-to-end Emergency Room (ER) Performance Dashboard built using Excel, Power Query, Power Pivot, and DAX.
This project delivers actionable insights to improve hospital efficiency, patient experience, and operational decision-making.



Problem Statement

Hospitals often struggle to track ER performance due to unstructured data, manual reporting, and lack of real-time visibility.

The objective of this project is to build a dynamic, automated Excel dashboard that helps stakeholders monitor key performance indicators such as:

Patient volume

Wait time

Satisfaction

Timeliness

Referral patterns


This enables faster and more accurate data-driven decisions.




Step-by-Step Procedure

1. Business Requirement Gathering

Identified key KPIs and data points needed by hospital management.

Understood operational challenges and reporting needs.


2. Understanding the Dataset

Reviewed raw hospital ER data including:
Patient age, gender, wait time, satisfaction, admission status, referral departments, etc.




3. Data Import Using Power Query

Pulled raw data into Excel using Power Query.

Ensured auto-refresh capability for future data updates.



4. Data Cleaning & Quality Assurance

Removed duplicates, fixed formatting issues, standardized data types.

Ensured consistency before modeling.




5. Creating Calendar Table (Power Query)

A fully dynamic date table was created to support time-intelligence.

= List.Dates(#date(2023,01,01), 731, #duration(1,0,0,0))



6. Data Modeling with Power Pivot

Built relationships between fact table and calendar table.

Optimized the model for fast and accurate calculations.


7. DAX Calculations (Custom Columns)

Age Group Classification


=IF([Patient Age]>=70,"70-79",
IF([Patient Age]>=60,"60-69",
IF([Patient Age]>=45,"45-59",
IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",
IF([Patient Age]>=5,"05-14","0-4"))))))



Patient Timeliness Classification

=IF([Patient Waittime] < 30, "Within Time", "Delay")



8. Dashboard Structure & Pivot Table Creation

- Built pivot tables for each KPI.

- Structured components for clarity and user-friendly navigation.



9. Chart Development & Formatting

Created automated visuals including:

Admission Status (Admitted vs Not Admitted)

Age Distribution

Gender Breakdown

Timeliness % (patients seen within 30 minutes)

Department Referral Analysis

Sparkline trends for daily wait time, satisfaction, and patient volume


10. Final Dashboard Development

Integrated KPIs, charts, and slicers.

Applied clean formatting for a professional, hospital-ready view.

Ensured everything updates automatically when source data changes.




🔧 Tools & Techniques Used

Microsoft Excel

Power Query (Importing & Cleaning)

Power Pivot (Data Modeling)

DAX (Custom Calculations)

Pivot Tables

Charts & Visualizations

Dashboard Layout & UX Optimization




📐 Methods Applied

Data Transformation

ETL using Power Query

Data Modeling

DAX-Based Calculations

Trend Analysis

KPI Design

Visual Storytelling





🔑 Key Insights

Identified peak traffic days where wait times increased significantly.

Certain age groups showed higher admission rates.

Gender distribution remained balanced.

Timeliness metric revealed specific low-performance days.

Referral patterns highlighted departments with maximum incoming cases.





🎯 Result & Conclusion

The final Excel dashboard provides a clear, automated, and insight-driven view of ER performance.

Hospital administrators can now:

Identify inefficiencies quickly

Track performance trends instantly

Make accurate, data-backed decisions

Improve patient experience and service quality




Contact

Krishna Jaiswal
📩 Email: krishna250763@gmail.com
🔗 LinkedIn: www.linkedin.com/in/krishnaa07
