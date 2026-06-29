# RFM Unsupervised Learning Project

## Project Overview
This project analyzes a UK-based online retail dataset using RFM (Recency, Frequency, Monetary) analysis and unsupervised learning techniques. The goal is to segment customers based on purchasing behavior, identify patterns in the sales data, and provide business recommendations.

## Dataset
The dataset contains sales transaction records for a London-based online retailer from 2007 to 2008. The store sells gifts and homeware products to individual customers and small businesses worldwide.

- Dataset source: https://archive.ics.uci.edu/ml/datasets/online+retail

## Dashboard
A visual report is available to summarize the analysis and key findings.

- Dashboard link: https://datastudio.google.com/reporting/bd5637de-5531-4362-b77c-93a9bdb17a3c
<img width="1910" height="1316" alt="image" src="https://github.com/user-attachments/assets/dae44cab-287e-4611-ba7c-57a99ae85c78" />


## Key Features
- `InvoiceNo`: transaction identifier; invoice numbers beginning with `C` indicate cancellations.
- `StockCode`: product identifier.
- `Description`: product name.
- `Quantity`: number of items sold; negative values indicate returned or cancelled orders.
- `InvoiceDate`: transaction date.
- `UnitPrice`: product price per unit in pounds sterling (£).
- `CustomerID`: customer identifier.
- `Country`: customer country.

## Methodology
The notebook performs the following steps:
1. Data inspection and cleaning.
2. Handling missing values by removing records without `CustomerID`.
3. Feature engineering, including creation of `TotalCost` and transaction date fields.
4. Preparing a binary target label for order cancellation.
5. Building the RFM model:
   - Recency: days since last purchase.
   - Frequency: number of transactions per customer.
   - Monetary: total spending per customer.
6. Applying clustering and unsupervised learning to identify customer segments.
7. Exploring sales trends, product popularity, and customer revenue contribution.

## Objective
- Discover customer segments using RFM and clustering.
- Analyze sales trends over time.
- Understand product purchase patterns.
- Evaluate customer contributions to revenue.
- Provide strategic business recommendations based on cluster behavior.
- Demonstrate a supervised classification approach for predicting cancelled orders.

## Notes
The notebook uses a Google Colab environment and expects the dataset file to be loaded from Google Drive.
