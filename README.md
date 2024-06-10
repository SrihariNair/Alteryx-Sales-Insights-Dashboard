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

## Workflow Data Flow

**Data Flow Description**
This section details the streamlined process of our Alteryx workflow, which efficiently manages data through several key stages to generate insights on top customer transactions:

1. **Data Importation**:
    - Data is loaded from `Customers.csv` for demographics and responses, and `Transactions.xml` for transaction details, using Alteryx's Input Data tool.

2. **Data Filtering**:
    - The Filter tool in Alteryx is used to exclude customers who responded with 'No', ensuring the analysis focuses only on engaged customers.

3. **Data Joining and Aggregation**:
    - Customer data is joined with transaction details using the Join tool, based on customer IDs.
    - The Summarize tool aggregates transaction amounts to calculate total sales per customer.

4. **Output Generation**:
    - Sorted data (by total sales) using the Sort tool identifies the top customers.
    - The top 10 customers by sales are extracted and compiled into `top_10_sales.xlsx` using the Output Data tool.

## Tools Used
- **Alteryx Designer**: Used to design and execute the data processing workflow.

## Getting Started
- Download and install Alteryx Designer.
- Open the provided workflow file (.yxmd) in Alteryx Designer.
- Run the workflow to process the data and generate the output.

## Contributing
If you have suggestions for improving the workflow, please fork this project, make your changes, and submit a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
