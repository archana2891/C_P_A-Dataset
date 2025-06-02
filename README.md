📁 Dataset Overview
This Dataset focuses on cleaning and preparing a raw Excel dataset for analysis. The dataset required attention to missing values, inconsistent date formats, unstructured headers, and incorrect data types. All transformations were performed using Microsoft Excel features such as filters, formulas, formatting tools, and data validation.

🧼 Data Cleaning Steps
1. 🔍 Initial Inspection
Opened the raw Excel file and reviewed the data layout.

Identified anomalies such as blank cells, incorrect column headers, and inconsistent formats.

2. ❌ Handling Missing Values
Used Excel filters to locate empty cells.

Strategies applied:

Deleted rows with large amounts of missing data.

Used formulas like =IF(ISBLANK(cell), "N/A", cell) to flag or fill missing cells.

Applied forward fill or manual imputation where appropriate.

3. 🗓️ Cleaning and Formatting Date Columns
Identified non-standard date formats or mixed date types.

Used:

TEXT(cell, "YYYY-MM-DD") to standardize format.

DATEVALUE() to convert text-based dates into Excel-recognized dates.

Corrected cells that had dates stored as text or numbers.

4. 🏷️ Cleaning and Renaming Headers
Removed extra rows above headers (e.g., metadata or notes).

Renamed headers to be consistent, concise, and meaningful.

Ensured no merged cells in header rows and removed special characters or extra spaces using TRIM().

5. 🔄 Data Type Correction
Ensured:

Dates were formatted using Date cell format.

Numeric columns had Number or Currency formatting.

Text/categorical data was set to Text format.

Used Data > Text to Columns where needed to split improperly combined data.

💾 Final Output
Cleaned Excel file saved as: cleaned_dataset.xlsx

The data is now:

Free from major missing values.

Contains clean and consistent headers.

Dates and numbers correctly formatted.

Ready for analysis or export to other tools (e.g., Python, Power BI, Excel PivotTables).
