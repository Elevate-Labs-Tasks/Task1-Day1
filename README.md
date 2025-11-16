# Task1-Day1
Task 1 – Data Cleaning and Preprocessing (Handling nulls, duplicates, formatting, datatype fixes, cleaned dataset)
Data Cleaning Report

Input file: marketing_campaign.csv
Detected delimiter: '\t'
Original shape (rows, cols): (2240, 29)
Final shape (rows, cols): (2215, 30)

Columns dropped due to >50% missing: None
Total rows removed for missing critical columns: 24

Numeric conversions attempted on: year_birth, income, mntwines, mntfruits, mntmeatproducts, mntfishproducts, mntsweetproducts, mntgoldprods, numdealspurchases, numwebpurchases, numcatalogpurchases, numstorepurchases, numwebvisitsmonth, z_costcontact

Date parsing info:
 - dt_customer: dayfirst=True

Top missing counts after cleaning (top 20):
 - id: 0
 - year_birth: 0
 - education: 0
 - marital_status: 0
 - income: 0
 - kidhome: 0
 - teenhome: 0
 - dt_customer: 0
 - recency: 0
 - mntwines: 0
 - mntfruits: 0
 - mntmeatproducts: 0
 - mntfishproducts: 0
 - mntsweetproducts: 0
 - mntgoldprods: 0
 - numdealspurchases: 0
 - numwebpurchases: 0
 - numcatalogpurchases: 0
 - numstorepurchases: 0
 - numwebvisitsmonth: 0

Notes:
 - Trimmed & normalized headers to lowercase underscore style.
 - Standardized education, marital_status, gender when present.
 - Created 'age' from year_birth (if present).
 - Removed obvious impossible values (age<0 or >120, negative income).

Files produced:
 - cleaned_marketing_campaign.csv
 - reports\summary.txt
