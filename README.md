# Alteryx Sales Insights Dashboard

## Project Overview
This project employs an Alteryx workflow to process and analyze customer and transactional data. The primary aim is to identify significant transaction patterns and top customers based on sales volume. The output is a detailed report highlighting the top customer transactions.

## Data Sources
- `Customers.csv`: Contains demographic data and customer response status.
- `Transactions.xml`: Includes detailed customer transaction records.

## Workflow Description
1. **Data Loading**: Import data from `Customers.csv` and `Transactions.xml`.
2. **Data Filtering**: Filter out records where customers have responded with 'No'.
3. **Data Processing**:
   - Join the customer data that has been filtered with transaction data based on customer IDs.
   - Aggregate transactions to compute the total sales for each customer.
4. **Output Generation**:
   - Customers are sorted by their total sales in ascending order.
   - The top 10 customers by sales are extracted and detailed in the `top_10_sales.xlsx` file.

## Tools Used
- **Alteryx Designer**: Used to design and execute the data processing workflow.

## Getting Started
- Download and install Alteryx Designer.
- Open the provided workflow file (.yxmd) in Alteryx Designer.
- Run the workflow to process the data and generate the output.

## Contributing
If you have suggestions for improving the workflow, please fork this project, make your changes, and submit a pull request.
