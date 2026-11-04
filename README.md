# Data & AI Job Postings: Europe, US & Canada

A point-in-time dataset of **107,102 curated job postings** across Europe, Canada, and the United States. It includes normalized job families, extracted skills, salary information, experience, seniority, and work-arrangement metadata.

## Explore the dashboard

The [DataTalent dashboard](https://datalent.pages.dev/) is the interactive companion to this dataset, visualizing job-market patterns across roles, skills, salaries, experience, and work arrangements. Use the dashboard to explore trends interactively, or download the CSV and Parquet files here to make your own analysis. The dashboard and this snapshot may differ in date coverage and filters.

## Files

- `data_ai_job_postings.csv`
- `data_ai_job_postings.parquet`

Both files contain the same records and columns. Parquet is recommended for analysis; the CSV is provided for convenience.

## Coverage and date handling

This snapshot was prepared on **2026-10-30**. The `posted_at` field has **month-level precision** (`YYYY-MM`), covering May through October 2026.

## Data schema

| Field | Description |
|---|---|
| `job_id` | Opaque job identifier |
| `posted_at` | Posting month (`YYYY-MM`) |
| `job_family` | Normalized job family |
| `country_code` | Country code |
| `salary_min`, `salary_max` | Salary range where available |
| `currency` | Salary currency; values may differ across records |
| `yoe` | Required years-of-experience information, where available |
| `seniority` | Seniority category, where available |
| `extracted_skills` | Extracted skills, serialized as a JSON array |
| `job_presence` | Work-arrangement category |
| `office_days_per_week` | Office days per week, where available |
| `company_size` | Company-size category, where available |
| `business_sector` | Business-sector category, where available |

## Excerpt of the dataset

| Job ID | Posted | Country | Job Family | Salary Range | YOE | Seniority | Work Arrangement | Company Size | Sector | Skills |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| `b4c...a7b` | 2026-10-09 | GB | AI Engineer | £70,000–£90,000 | 2–4 | — | Hybrid | 1–10 | Information Technology | Azure ... scikit-learn |
| `cce...909` | 2026-09-04 | PT | Data Engineer | €43,000–€53,000 | 5–7 | Senior | Remote | 100–500 | Information Technology | Agile ... Scrum |
| `674...134` | 2026-08-25 | GB | Data Analyst | £45,000–£55,000 | 5–7 | Senior | Hybrid | 100–500 | Industrials | Power BI ... SQL |
| `5fb...ccb` | 2026-09-04 | PL | Data Scientist | 261,600–302,400 PLN | 5–7 | — | Remote | 501–1000 | Information Technology | ETL/ELT ... Spark |
| `368...097` | 2026-08-02 | FR | AI Engineer | €75,000–€95,000 | 5–7 | Principal/Lead | Hybrid | 11–50 | Communication Services | Computer Vision ... Python |
| `d58...62d` | 2026-08-26 | US | Data Scientist | $170,000–$170,000 | 2–4 | — | Remote | — | — | Databricks ... Statistics |
| `c06...ad3` | 2026-07-17 | US | ML Engineer | $99,600–$192,900 | 5–7 | — | Hybrid | — | — | Agile ... XGBoost |
| `084...8a9` | 2026-08-18 | US | AI Engineer | $85,000–$122,200 | 2–4 | — | Hybrid | 100+ | Consumer Staples | Agile ... SQL |
| `393...2be` | 2026-08-13 | US | Data Analyst | $130,000–$175,000 | 5–7 | Senior | Hybrid | 100–500 | Information Technology | CI/CD ... dbt |
| `19b...23a` | 2026-09-28 | US | Data Engineer | $118,000–$164,800 | 2–4 | Principal/Lead | Remote | 100+ | Financials | AWS ... Snowflake |

## Limitations

This is a curated snapshot, not a complete census of job openings. Coverage depends on the sources and collection process. Salary values and other fields may be missing.

This release contains no job descriptions, employer names, or job URLs.

## Source terms and user responsibilities

This dataset contains transformed job-level attributes derived from job listings on third-party websites. Source-platform names, listing URLs, job titles, employer names, and descriptions have been omitted. Applicable terms and third-party rights have not been verified; public accessibility does not necessarily permit collection or redistribution. This dataset is independent and is not endorsed by those websites. Please check applicable terms before using or sharing it.
