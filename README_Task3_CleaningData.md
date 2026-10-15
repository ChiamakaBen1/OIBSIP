# OASIS INFOBYTE — Data Analytics Level 1, Task 3: Cleaning Data

## Project goal
Clean the supplied cafe sales dataset, document each decision, inspect outliers with IQR, compare data quality before and after, and save a new CSV.

## Files
- `dirty_cafe_sales.csv` — original dataset (keep unchanged)
- `OIBSIP_DataAnalytics_L1_Task3_CleaningData.ipynb` — documented notebook with code and explanations
- `cleaned_cafe_sales.csv` — cleaned output
- `cafe_data_quality_summary.csv` — before/after summary

## Key decisions
- Converted `UNKNOWN` and `ERROR` placeholders to missing values before cleaning.
- Converted Quantity, Price Per Unit, and Total Spent to numeric types; parsed Transaction Date as a date.
- Used observed consistent prices for recognised items to fill missing unit prices.
- Recovered a missing quantity only when Total Spent divided by Price Per Unit gave an exact whole number between 1 and 5.
- Recalculated missing totals as Quantity × Price Per Unit when both inputs were available.
- Removed rows only where quantity remained unknown and could not be recovered.
- Replaced missing/invalid category labels with `Unknown Item` or `Not recorded`.
- Used the IQR method to flag outliers. Flagged values were reviewed, not automatically deleted.
- Left dates and some prices/totals blank when they could not be reliably inferred.

## Results
- Rows before cleaning: 10000
- Rows after cleaning: 9977
- Rows removed due to unrecoverable quantity: 23
- Exact duplicate rows before cleaning: 0
- Exact duplicate rows after cleaning: 0

## How to run
Place the original `dirty_cafe_sales.csv` in the same folder as the notebook, open the notebook in Jupyter Notebook or Google Colab, and run the cells from top to bottom.
