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

## Fields

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

## Limitations

This is a curated snapshot, not a complete census of job openings. Coverage depends on the sources and collection process. Salary values may be missing, and different currencies should not be compared without conversion.

This release contains no job descriptions, employer names, or job URLs.

## Source terms and user responsibilities

This dataset contains transformed job-level attributes derived from job listings on third-party websites. Source-platform names, listing URLs, job titles, employer names, and descriptions have been omitted. Applicable terms and third-party rights have not been verified; public accessibility does not necessarily permit collection or redistribution. This dataset is independent and is not endorsed by those websites. Please check applicable terms before using or sharing it.
