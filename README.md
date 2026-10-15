# Exploratory Data Analysis (EDA) on Retail Sales Data

## Project Overview
This project explores a retail sales dataset to understand sales activity, customer demographics, and product-category performance. The analysis is intended to identify patterns in the data and turn them into practical business recommendations.

## Dataset
The file used for this project is `retail_sales_dataset.csv`.

The dataset contains **1,000 rows and 9 columns**:

- `Transaction ID` — identifier for each transaction
- `Date` — date of the transaction
- `Customer ID` — identifier for the customer
- `Gender` — customer gender
- `Age` — customer age
- `Product Category` — category of the purchased product
- `Quantity` — number of units purchased
- `Price per Unit` — price per unit
- `Total Amount` — total amount for the transaction

An initial check of the supplied CSV found no missing values. The `Date` column is stored as text in the original file and should be converted to a date/time type in Python before carrying out monthly or quarterly trend analysis.

## Tools and Libraries
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Analysis
Use this section to describe the analyses actually completed in your notebook. Depending on your completed work, this may include:

- Initial dataset inspection and data-quality checks
- Descriptive statistics for numerical columns
- Monthly and quarterly sales trends
- Customer age and gender analysis
- Best-selling products and revenue by product category
- Correlation heatmap for numerical variables
- An additional visualisation to uncover another useful pattern

## Key Findings
Add the main findings from your own charts and calculations here. Make sure each finding is supported by the results in your notebook. Avoid adding conclusions that your analysis did not establish.

1. **Finding 1:** [Write a finding from your results.]
2. **Finding 2:** [Write a finding from your results.]
3. **Finding 3:** [Write a finding from your results.]

## Business Recommendations
Include at least **three specific, actionable recommendations** based on your findings.

1. **Recommendation 1:** [State what the business should do and which finding supports it.]
2. **Recommendation 2:** [State what the business should do and which finding supports it.]
3. **Recommendation 3:** [State what the business should do and which finding supports it.]

## How to Run the Notebook
1. Download or clone the project folder.
2. Make sure Python and Jupyter Notebook are installed.
3. Install the required libraries if needed:

   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

4. Open Jupyter Notebook and open the `.ipynb` file for this project.
5. Ensure `retail_sales_dataset.csv` is in the same folder as the notebook, or update the dataset path in the code.
6. Run the notebook cells in order.

## Project Files
A suggested folder structure is:

```text
OIBSIP/
└── DataAnalytics-L1-EDARetailSales/
    ├── README.md
    ├── EDA_Retail_Sales.ipynb
    └── retail_sales_dataset.csv
```

Include any relevant screenshots or output files if they help demonstrate your work.

## Notes
This README describes the supplied dataset and provides sections for your own results. Before submitting, replace the bracketed placeholders in **Key Findings** and **Business Recommendations** with the actual findings and recommendations from your completed notebook.
