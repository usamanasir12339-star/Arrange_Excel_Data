for use this tool website link is here 
https://business-analytics-tool-hlxsanyaygepnqm3nfbaft.streamlit.app/#key-numbers





# Business Analytics Tool

A simple web app for business users. Upload a CSV or Excel file and get an automatic dashboard with key numbers, charts and a data quality report. No technical setup or settings needed.

**Live demo:** PASTE YOUR LIVE LINK HERE
(The app may take up to a minute to wake up if it has not been opened for a while.)

**Flow:** Upload file → Automatic analysis → Dashboard

## What it does (Version 1.1)

- Reads `.csv` and `.xlsx` files (up to 20 MB) and shows friendly messages for problem files
- Finds columns automatically, even when names differ (Sales, Revenue, Amount, Cost, Expenses, Profit, Date, Product, Customer, Category, Department, Quantity, Supplier, Employee)
- Shows key numbers only when the data exists: Total Revenue, Expenses, Profit, Profit Margin, Quantity Sold
- Monthly trend chart, plus top-10 revenue charts by product, category and department
- Data quality report in plain language: empty cells, duplicate rows, invalid dates, text in number columns, negative values
- "Try with sample data" button to explore without a file

## How profit is calculated

If the file has a Profit column, that column is used. If not, Profit = Revenue minus Expenses, and the app says so.

## Privacy

Uploaded files are processed only during your session. This app does not save them.

## Sample data

`sample_business_data.csv` is demo data made for testing. It is not real business data. It contains a few deliberate problems (a duplicate row, an empty customer, an invalid date) so the data quality checks can be seen working.

## Run it on your own computer

1. Install Python
2. Install the packages: `pip install -r requirements.txt`
3. Start the app: `streamlit run app.py`

## Built with

Python, Streamlit, Pandas, OpenPyXL

## Not built yet

- Interactive filters (date, product, department, customer)
- Automatic written business insights
- Downloadable summary report (Excel / PDF)

## About

Built by YOUR NAME, BBA (Hons) student, as a practical business analytics project.
