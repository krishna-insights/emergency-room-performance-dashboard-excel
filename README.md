Emergency Room Performance Dashboard (Excel)

A complete end-to-end Emergency Room (ER) Performance Dashboard built using Excel, Power Query, Power Pivot, and DAX.
This project delivers actionable insights to improve hospital efficiency, patient experience, and operational decision-making.




📌 Problem Statement

Hospitals struggle to track ER performance due to:

- Unstructured data

- Manual reporting

- Lack of real-time visibility


This project helps stakeholders monitor essential ER KPIs such as:

- Patient volume

- Wait time

- Satisfaction

- Timeliness

- Referral patterns





🛠️ Step-by-Step Procedure

1. Business Requirement Gathering

- Identified key KPIs needed by hospital management.

- Understood operational challenges and reporting needs.



2. Understanding the Dataset

- Reviewed raw hospital ER data including:

- Patient demographics

- Wait time

- Satisfaction

- Admission status

- Referral departments



3. Data Import Using Power Query

- Pulled raw data into Excel using Power Query.

- Enabled auto-refresh for future updates.



4. Data Cleaning & Quality Assurance

- Removed duplicates

- Fixed formatting issues

- Standardized data types

- Ensured consistency before modeling



5. Creating Calendar Table (Power Query)

= List.Dates(#date(2023,01,01), 731, #duration(1,0,0,0))



6. Data Modeling with Power Pivot

- Built relationships between fact and calendar tables.

- Optimized model for fast and accurate calculations.



7. DAX Calculations

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

- Created user-friendly layout with structured components.



9. Chart Development & Formatting

- Created automated visuals including:

- Admission status

- Patient satisfaction

- Referral trends

- Patient age distributions

- Timeliness performance




📈 Key Insights

- Identified delays in patient processing

- Found bottlenecks in specific departments

- Highlighted age groups with highest ER visits

- Improved data refresh workflow

  




✅ Result & Conclusion

This dashboard provides:

- Transparent performance tracking

- Faster decision-making

- Improved patient experience

- Scalable solution for future datasets






📦 Tools & Technologies Used

- Excel

- Power Query

- Power Pivot

- DAX

- Data Cleaning & Modeling

- DAX-Based Calculations

- Trend Analysis

- KPI Design

- Visual Storytelling





🔑 Key Insights

- Identified peak traffic days where wait times increased significantly.

- Certain age groups showed higher admission rates.

- Gender distribution remained balanced.

- Timeliness metric revealed specific low-performance days.

- Referral patterns highlighted departments with maximum incoming cases.





🎯 Result & Conclusion

The final Excel dashboard provides a clear, automated, and insight-driven view of ER performance.

Hospital administrators can now:

- Identify inefficiencies quickly

- Track performance trends instantly

- Make accurate, data-backed decisions

- Improve patient experience and service quality




Contact

Krishna Jaiswal  
📩 Email: krishna250763@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/krishnaa07
