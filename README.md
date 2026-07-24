# SQL Data Cleaning & EDA: Tech Layoffs Dataset

## Dataset
Dataset from Alex the Analyst's SQL bootcamp series (MySQL-YouTube-Series GitHub repo), originally sourced from Kaggle's "Layoffs 2022" dataset.
~2,361 rows of company layoff records (company, industry, country, total laid off, date, funds raised, etc.)

## What I Did
I cleaned a raw dataset of tech company layoffs using SQL, then explored it to uncover patterns. Cleaning involved creating a staging table to protect the raw data, removing duplicate records, standardizing inconsistent values, and handling nulls. I then ran exploratory queries to look at layoffs by company, industry, country, and year, including a ranking query to find the top 3 companies with the most layoffs each year, and a rolling monthly total of layoffs over time.

## Key Steps
- Created a staging table to preserve original raw data
- Removed duplicate rows
- Standardized inconsistent company, industry, and country names
- Handled NULL and blank values
- Queried layoffs by company, location, country, industry, and company stage
- Used DENSE_RANK() with CTEs to find the top 3 companies with the highest layoffs per year
- Calculated a rolling monthly total of layoffs using window functions

## Key Findings
- Amazon had the highest total layoffs (18,150), followed by Google (12,000), Meta (11,000), Salesforce (10,090), and Microsoft (10,000)
- Consumer was the hardest-hit industry (46,682 layoffs), followed closely by Retail (43,613) and "Other" (36,289)
- 2022 was the worst year for layoffs (161,711 total), nearly double the 2020 pandemic-year total (81,068), with 2023 continuing the trend at 127,277

## Tools
MySQL, GitHub Desktop

## Files
- `01_data_cleaning.sql`
- `02_exploratory_analysis.sql`
- `layoffs.csv` — raw dataset
