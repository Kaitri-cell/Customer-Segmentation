# Customer-Segmentation
Customer Segmentation and Retail Sales Analysis
A customer segmentation project built with Orange Data Mining and the UCI Online Retail dataset. The workflow prepares transaction data, creates customer-level RFM features, applies K-Means clustering, and supports visual inspection and interpretation of the resulting customer groups.

Project goals
- Explore purchasing behavior in a UK-based online retail dataset.
- Summarize customer behavior with Recency, Frequency, and Monetary (RFM) features.
- Group customers with K-Means to support customer profiling and possible marketing and retention decisions.

Dataset
This project uses the Online Retail dataset from the UCI Machine Learning Repository. It contains transaction records with fields such as invoice number, product, quantity, invoice date, unit price, customer ID, and country.
Download the dataset from UCI and select it in the File widget when opening the Orange workflow. The source dataset is not included in this repository.
Method
The Orange workflow shown in this project follows these main stages:
1. Load and inspect the transaction data.
2. Preprocess records and select the rows used in the analysis.
3. Create transaction-level values and aggregate transactions by customer.
4. Build customer-level RFM features:
   - Recency: time since the customer's most recent purchase.
   - Frequency: number of purchases or invoices.
   - Monetary: total spending, calculated from quantity and unit price and aggregated per customer.
5. Prepare the RFM data for clustering, including preprocessing and feature selection.
6. Apply K-Means and inspect the clusters with Orange's Scatter Plot, Silhouette Plot, and Box Plot widgets.
7. Summarize cluster profiles and assign interpretable segment names.
In the exploratory comparison, k = 6 was examined because it showed no negative silhouette scores among the tested options. The final choice of cluster count should also consider cluster sizes, separation, and whether the profiles are useful to interpret.

Tools
- Orange Data Mining
- K-Means clustering
- RFM analysis
- Silhouette Plot, Scatter Plot, and Box Plot visualizations



