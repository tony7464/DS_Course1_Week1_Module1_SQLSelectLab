# Requirements Checklist: 44946 Lab: Getting Started with Databases and SQL

Source: Canvas description + rubric (latest_assignments.json), plus the starter notebook/repo instructions.

Deliverable: `SQLSelectLab.ipynb`

| # | Requirement (explicit or implied) | Rubric criterion | How it's met | Status |
|---|---|---|---|---|
| 1 | Step 1: import sqlite3 + pandas (pd alias), `conn` to data.sqlite | Rubric: Connecting to Data (5) | `conn = sqlite3.connect('data.sqlite')` | ✅ |
| 2 | Step 2: employeeNumber, lastName only | Basic Select Filtering (10) | `df_name_number`, 2 columns, 23 rows | ✅ |
| 3 | Step 3: lastName before employeeNumber | Basic Select Filtering | `df_reverse` | ✅ |
| 4 | Step 4: alias employeeNumber AS ID | Aliasing in Select (10) | `df_alias` columns lastName, ID | ✅ |
| 5 | Step 5: CASE -> role Executive / Not Executive (President, VP Sales, VP Marketing) | CASE Function (10) | `df_executive` with `role` column | ✅ |
| 6 | Step 6: length(lastName) AS name_length only | Built-In Functions: Strings (10) | `df_name_length` single column | ✅ |
| 7 | Step 7: substr(jobTitle,1,2) AS short_title only | Built-In Functions: Strings | `df_short_title` single column | ✅ |
| 8 | Step 8: SUM of ROUND(priceEach*quantityOrdered) | Built-In Functions: Numerics (5) | `sum_total_price` = 9,604,251.0 (rounded inside the query, then .sum()) | ✅ |
| 9 | Step 9: orderDate + day, month, year columns | Built-In Functions: Numerics | `df_day_month_year` via strftime on orders.orderDate | ✅ |
| 10 | Keep provided 'run without changes' cells, close conn | implied | unchanged | ✅ |
| 11 | Notebook executes top to bottom with no errors | implied (CodeGrade) | `jupyter nbconvert --execute` passed | ✅ |
| 12 | Comments explaining each query | quality | every solution cell commented | ✅ |
