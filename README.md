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


# Data Analysis on Job Postings - Power BI Visualizations

## Overview

This repository showcases the data analysis conducted on job postings using Excel and Power BI. The analysis provides valuable insights into optimal hiring periods, strategic hiring locations, salary distributions, and effective marketing and regulation strategies.

## Power BI Visualizations

### When to Hire?(pg1)
![Image Alt Text](Img/Screenshot%202024-01-11%20at%2012.21.33%20PM.jpeg)

1. **Count of Job ID / Date posted on**
   - Understand the fluctuations in job postings and determine the optimal times for posting jobs to enhance profit margins.
2. **Count of Job / Job Title**
   - Gain insights into the demand for each job and the trends in job titles over the years, complementing the Count of Job ID / Date posted graph.
3. **Slicer graph**
   - Use the slicer graph to dynamically filter job postings between 2021 and 2023.

### Where to Hire?(pg2)
![Skills / Location Visuals](Img/Screenshot%202024-01-11%20at%2012.24.32%20PM.jpeg)

1. **Skills / Location**
   - Analyze skill demand in each country, enabling strategic hiring decisions based on skill availability and demand.
2. **Status/Count Job ID**
   - Utilize a graph to infer the number of companies currently hiring, providing insights for further analysis.
3. **Year posted on**
   - Employ a slicer graph to filter job postings by each year, facilitating temporal trend analysis.

### What Salary to Offer?(pg3)
![Salary Distribution Visuals](Img/Screenshot%202024-01-11%20at%2012.23.25%20PM.jpeg)

1. **Salary Distribution / Location Clubbed with Industry / Count of Job : (pg3)**
   - Understand salary distribution across industries and locations, aiding decisions on industry-specific hiring and salary offerings.
2. **Average salary and average max salary by date posted on**
   - Observe salary trends over time, crucial for determining competitive salary structures.
3. **Status**
   - Dynamically filter hiring or static job postings for a detailed analysis.

### What Marketing & Regulation?(pg4)
![Marketing & Regulation Visuals](Img/Screenshot%202024-01-11%20at%2012.23.34%20PM.jpeg)

1. **Average salary and count of job ID by Rating**
   - Leverage company ratings for effective marketing strategies and attracting high-caliber employees.
2. **Average salary and count of job ID by Rating - Scatter Chart Clubbed with Job Count / Job Type**
   - Estimate competitive salaries to maintain or improve company ratings, ensuring a favorable profit margin.
3. **Average of Rating and First Size by Company Name**
   - Explore competitors with similar ratings, providing insights for strategic adjustments and enhanced market standing.

## Business Recommendations

The analysis equips the company with data-driven insights for effective hiring strategies, ensuring a competitive position in the job market. The combination of Excel for data processing and Power BI for visualization offers a comprehensive approach to analyzing job postings data.

