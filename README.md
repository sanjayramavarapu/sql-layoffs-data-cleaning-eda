# Global Layoffs Data Cleaning & Analysis (SQL)

## Project Overview

This project focuses on cleaning and analyzing a global layoffs dataset using SQL.
The goal is to transform raw data into a structured dataset and perform exploratory data analysis to identify trends in layoffs across companies, industries, and time periods.

The project demonstrates practical SQL skills including data cleaning, duplicate removal, handling missing values, and performing analytical queries.

## Dataset

The dataset contains information about company layoffs including:

* Company name
* Industry
* Location
* Total employees laid off
* Percentage of workforce laid off
* Funding raised
* Company stage
* Layoff date

## Tools Used

* MySQL
* SQL Window Functions
* Aggregation Functions
* Date Functions

## Data Cleaning Process

The dataset was cleaned using a structured SQL pipeline:

### 1. Creating a Staging Table

A staging table was created to safely clean and transform the raw dataset without modifying the original data.

### 2. Removing Duplicate Records

Duplicates were identified using the `ROW_NUMBER()` window function and removed from the dataset.

### 3. Standardizing Data

Data inconsistencies were corrected using SQL string functions:

* Trimmed company names
* Standardized industry names
* Normalized country values

### 4. Converting Date Formats

Text-based dates were converted into SQL date format using `STR_TO_DATE()` to enable time-based analysis.

### 5. Handling Missing Values

Missing values were addressed by:

* Identifying null or blank records
* Using self-joins to populate missing industry fields
* Removing rows with insufficient information

## Exploratory Data Analysis

After cleaning the dataset, several analytical queries were performed:

### Key Analyses

* Companies with the highest layoffs
* Industries most affected by layoffs
* Yearly layoffs trends
* Monthly layoffs patterns
* Companies with complete workforce layoffs

### SQL Techniques Used

* `GROUP BY`
* Aggregation functions (`SUM`, `MAX`)
* Filtering with `WHERE`
* Date functions (`YEAR`, `SUBSTRING`)
* Sorting and ranking

## Example Insights

The analysis helped identify:

* Companies responsible for the largest layoffs
* Industries with the highest workforce reductions
* Changes in layoff trends over time
* Months with peak layoffs activity

## Learning Outcomes

* Building SQL-based data cleaning pipelines
* Using window functions for duplicate detection
* Handling missing and inconsistent data
* Performing exploratory data analysis with SQL
* Extracting meaningful insights from structured datasets
