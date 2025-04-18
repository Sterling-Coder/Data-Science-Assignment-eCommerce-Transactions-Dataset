# Data Science Assignment: eCommerce Transactions Dataset

This repository contains my solution to the eCommerce Transactions Dataset analysis assignment, which includes exploratory data analysis, customer segmentation, and a lookalike customer model.

## Assignment Overview

The assignment involves analyzing an eCommerce transaction dataset to perform:
1. Exploratory data analysis with business insights
2. Building a lookalike customer model 
3. Customer segmentation using clustering techniques

## Datasets

The analysis uses three primary datasets located in the `DataSets` directory:

1. **Customers.csv**: Contains customer information with fields:
   - CustomerID: Unique identifier for each customer (format: C####)
   - CustomerName: Name of the customer
   - Region: Geographic region (North America, South America, Europe, Asia)
   - SignupDate: Date when the customer signed up

2. **Products.csv**: Contains product information with fields:
   - ProductID: Unique identifier for each product (format: P###)
   - ProductName: Name of the product
   - Category: Product category (Books, Electronics, Home Decor, Clothing)
   - Price: Product unit price

3. **Transactions.csv**: Contains transaction data with fields:
   - TransactionID: Unique identifier for each transaction (format: T#####)
   - CustomerID: Identifier linking to the Customer dataset
   - ProductID: Identifier linking to the Product dataset
   - TransactionDate: Date and time of transaction
   - Quantity: Number of units purchased
   - TotalValue: Total monetary value of the transaction
   - Price: Unit price of the product

## Solution Components

### 1. Task 1: Exploratory Data Analysis (EDA) and Business Insights
- `Aman_Rastogi_EDA.ipynb`: Jupyter notebook containing exploratory analysis of the transaction data
- `Aman_Rastogi_EDA.pdf`: PDF report with business insights derived from the EDA

The EDA explores patterns in customer behavior, product performance, and transaction trends to extract actionable business insights.

### 2. Task 2: Lookalike Customer Model
- `Aman_Rastogi_Lookalike.ipynb`: Jupyter notebook implementing a similarity-based recommendation model
- `Aman_Rastogi_Lookalike.csv`: CSV output with top 3 lookalike customers for CustomerIDs C0001-C0020

The lookalike model identifies similar customers based on their profile and transaction history, assigning similarity scores to recommended customers.

### 3. Task 3: Customer Segmentation via Clustering
- `Aman_Rastogi_Clustering.ipynb`: Jupyter notebook with customer segmentation analysis
- `Aman_Rastogi_Clustering.pdf`: PDF report on clustering results, including metrics like DB Index

The clustering analysis segments customers based on both profile information and transaction history using appropriate clustering algorithms.

## Lookalike Model Details

The implemented lookalike model:
- Uses both customer profile and transaction information
- Features include geographic region (encoded), total spending behavior, and purchase quantity
- Calculates cosine similarity between customer feature vectors
- Identifies and ranks the top 3 most similar customers for each target customer
- Assigns a similarity score to each recommendation

## Clustering Approach

The customer segmentation:
- Utilizes both customer profile information and transaction history
- Implements appropriate clustering algorithms with optimal number of clusters
- Calculates clustering metrics including DB Index for evaluation
- Provides visualizations of the resulting customer segments

## Usage

To run the notebooks:
1. Ensure you have Python installed with required packages (pandas, numpy, scikit-learn, matplotlib, seaborn)
2. Open the Jupyter notebooks (.ipynb files) in JupyterLab or Jupyter Notebook
3. Run the cells sequentially to reproduce the analysis

## Key Insights

The analysis provides valuable business insights including:
- Customer purchasing patterns across different regions
- Product category performance and popularity trends
- Time-based transaction patterns
- Distinct customer segments with unique behavior profiles
- Similar customers for targeted marketing campaigns

## Evaluation Criteria

The assignment solutions were evaluated based on:
- Quality of exploratory data analysis (25%)
- Business insights derived from the data (15%)
- Lookalike model implementation and effectiveness (30%)
- Customer segmentation approach and results (30%) 