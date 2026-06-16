# LinkedIn Job Market Analysis using MySQL

## Project Overview

The job market is constantly evolving, and understanding hiring trends can provide valuable insights for job seekers, recruiters, and businesses. In this project, I analyzed a large dataset of LinkedIn job postings using MySQL Workbench to uncover patterns in hiring activity, salary distributions, remote work opportunities, and employment types.

The objective of this project was not only to practice SQL skills but also to demonstrate how real-world data can be transformed into actionable business insights. By working with thousands of job postings, I explored how organizations recruit talent, what types of positions dominate the market, and which roles offer the highest compensation.

This project highlights my ability to work with large datasets, perform data validation, write analytical SQL queries, and communicate findings effectively.

---

## Problem Statement

Organizations generate massive amounts of recruitment data every day, but raw datasets often provide little value without analysis.

This project aims to answer questions such as:

* Which companies posted the highest number of job openings?
* What is the average salary across the dataset?
* How common are remote work opportunities?
* Which employment types dominate the market?
* What roles appear to offer the highest compensation?
* Can unexpected hiring trends be identified through data?

---

## Dataset

### Source

Kaggle – LinkedIn Job Postings Dataset

### Dataset Characteristics

* Total records analyzed: **123,849 job postings**
* Total variables: **31 columns**
* Dataset format: CSV
* Imported and analyzed using MySQL Workbench

The dataset contains information such as:

* Job titles
* Company names
* Job descriptions
* Salary information
* Employment types
* Remote work availability
* Geographic identifiers
* Experience levels
* Application details
* Posting activity metrics

### Data Availability

The cleaned dataset used for analysis contains approximately **493 MB** of data, which exceeds GitHub's file size limitations.

Therefore, this repository includes:

* A sample dataset containing **1,000 records**
* SQL scripts used for analysis
* Python scripts used during preprocessing
* Screenshots of query outputs

This allows others to understand and reproduce the analysis workflow without requiring the full dataset.

---

## Tools and Technologies Used

### Database and Querying

* MySQL Workbench
* SQL

### Data Preparation

* Python
* Pandas

### Development Environment

* Visual Studio Code

### Version Control

* Git
* GitHub

---

## Project Workflow

### 1. Data Preparation

Before importing the dataset into MySQL, the CSV file was inspected and cleaned using Python.

Tasks included:

* Reviewing dataset dimensions
* Verifying column consistency
* Exporting a cleaned CSV file
* Generating a smaller sample dataset suitable for GitHub sharing

---

### 2. Database Creation

A MySQL database named:

```sql
linkedin_job_analysis
```

was created.

The postings table was designed with all 31 variables from the original dataset.

---

### 3. Data Import

The cleaned CSV file was imported into MySQL Workbench.

During this stage, several practical challenges were encountered and resolved, including:

* Duplicate column mappings
* Import wizard configuration issues
* Zero-row import errors
* Large file handling limitations

Resolving these issues provided valuable hands-on experience working with real-world datasets.

---

### 4. Exploratory SQL Analysis

SQL queries were written to answer business-oriented questions related to hiring activity and compensation trends.

---

## Key Insights

### Top Hiring Companies

One of the most surprising findings from the analysis was discovering which organizations had the highest hiring activity in the dataset.

| Rank | Company                                        | Number of Openings |
| ---- | ---------------------------------------------- | -----------------: |
| 🥇   | Liberty Healthcare and Rehabilitation Services |              1,108 |
| 🥈   | The Job Network                                |              1,003 |
| 🥉   | J. Galt                                        |                604 |
| 4️⃣  | TEKsystems                                     |                529 |
| 5️⃣  | Lowe's Companies, Inc.                         |                527 |

Rather than large technology companies dominating the rankings, the data revealed that healthcare organizations, staffing firms, recruiting platforms, and retail companies represented a substantial portion of hiring demand.

> **I expected tech giants to top the list. Instead, the data told a very different story.**

---

### Salary Insights

The average normalized salary across all available postings was:

## $59,799.71

The analysis also identified several roles associated with significantly higher salaries.

Many of these positions belonged to fields such as:

* Executive leadership
* Healthcare
* Legal services
* Engineering
* Specialized technical roles

These findings suggest that highly specialized expertise continues to command premium compensation.

---

### Remote Work Trends

Remote work opportunities accounted for only a minority of postings.

| Remote Status        | Number of Jobs |
| -------------------- | -------------: |
| On-site / Non-Remote |        108,603 |
| Remote Allowed       |         15,246 |

Approximately:

* **12.3%** of jobs supported remote work.
* **87.7%** required traditional work arrangements.

This highlights that despite the rise of remote employment, most opportunities in this dataset remained location-dependent.

---

### Employment Type Distribution

The job market was heavily dominated by full-time positions.

| Employment Type | Number of Jobs |
| --------------- | -------------: |
| Full-Time       |         98,811 |
| Contract        |         12,117 |
| Part-Time       |          9,695 |
| Temporary       |          1,190 |
| Internship      |            983 |
| Volunteer       |            562 |

This suggests that organizations continue to prioritize long-term employment relationships over short-term arrangements.

---

## SQL Skills Demonstrated

This project demonstrates proficiency in:

* Database creation
* Data importing and validation
* Aggregation functions (`COUNT`, `AVG`)
* Filtering using `WHERE`
* Grouping using `GROUP BY`
* Sorting using `ORDER BY`
* Result limiting using `LIMIT`
* Data quality assessment
* Exploratory data analysis
* Business insight generation
* Translating data into actionable findings

---

## Repository Structure

```text
linkedin-job-analysis/
├── data/
│   └── postings_sample.csv
├── sql/
│   ├── top_companies.sql
│   ├── average_salary.sql
│   ├── remote_jobs.sql
│   ├── work_types.sql
│   └── top_paying_jobs.sql
├── screenshots/
├── clean_postings.py
└── README.md
```

---

## Future Improvements

Potential extensions of this project include:

* Building an interactive dashboard using Power BI or Tableau.
* Performing geographic analysis of hiring trends.
* Conducting skill-demand analysis using job descriptions.
* Developing predictive models to estimate salaries.
* Automating the ETL pipeline for larger datasets.

---

## Conclusion

This project demonstrates how SQL can be applied to real-world business problems using large recruitment datasets. Beyond writing queries, the experience involved overcoming practical data challenges, validating results, and translating findings into meaningful insights.

The analysis reinforced an important lesson:

> Data often challenges our assumptions. The organizations hiring the most, the prevalence of remote work, and the distribution of salaries all told stories that differed from initial expectations.

---

## Author

### Anousha Gul

Aspiring Data Analyst passionate about transforming data into insights through SQL, Python, and analytics.

GitHub:
https://github.com/anoushagul4-web/linkedin-job-analysis
