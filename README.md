# Job Postings Data Analysis with Excel and Power BI

## Overview

This repository documents the analysis of job postings data over the years, utilizing Excel and Power BI. The analysis aims to understand the job market trends, optimize job postings, and make informed decisions about hiring strategies for the company.

## Data Cleaning and Processing

### Cleaning Data in Excel
- Removed index for clarity.
- Processed salary estimates to standardize and make them more meaningful.
- Converted "company founded" to "company age" for a more useful metric.
- Removed competitors' rows with insufficient data.

### Creating Tables and Metrics
- Developed tables of skills to identify demand in different areas.
- Determined job positions and seniority levels based on job titles.
- Implemented date-related metrics to analyze trends over time.


## Excel Formulas and Techniques Used

```excel
=SUBSTITUTE(C2, "$", "")  // Removing dollar signs from salary estimates
=VALUE(LEFT(C2, FIND("-", C2) - 1))  // Extracting minimum salary
=IF(ISNUMBER(SEARCH("Python", D2)), 1, 0)  // Creating a table of Python skills
=IF(ISNUMBER(SEARCH("data scientist", B2)), "data scientist", ...)  // Identifying job positions
=RANDBETWEEN(DATE(2021,1,1),DATE(2021,12,31))  // Generating random dates for analysis 
```


## Power BI Visualizations

### Key Visualizations and Insights

1. **Skills/Location Analysis (Page 1)**
   - Examined skill demand in each country to inform benefit offerings.
   - Used a status/count graph to understand the current job market.

2. **When to Hire? (May – Jul) (Page 2)**
   - Analyzed job posting trends to determine optimal hiring periods.
   - Utilized graphs for job counts, posting dates, and job titles.

3. **Salary Distribution/Location (Page 3)**
   - Explored salary distribution across industries and locations.
   - Created stacked area charts for average salary trends.

## Business Recommendations (Pages 4-5)

Img/Screenshot 2024-01-11 at 12.21.33 PM.jpeg

This analysis equips the company with data-driven insights for effective hiring strategies, ensuring competitive positioning in the job market.

The combination of Excel for data processing and Power BI for visualization offers a comprehensive approach to analyzing job posting data.

