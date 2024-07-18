# Market-Basket-Analysis
This market basket analysis project aims to uncover patterns and relationships between items frequently purchased together in an online retail dataset. The process includes:

Data Loading and Cleaning:

Dataset: Loaded from an Excel file containing 541,909 rows and 8 columns.
Cleaning: Removed rows with missing descriptions and customer IDs.
Handling Cancellations: Filtered out canceled transactions (InvoiceNo containing 'C').
Preprocessing: Removed extra white spaces in descriptions and converted invoice numbers to string format.
Country Focus:

Segmentation: Analyzed transactions across 38 countries.
Focus on Germany: Filtered data to include only transactions from Germany.
Transaction Encoding:

Grouping: Grouped transactions by invoice number and item description, then counted item occurrences.
Binary Conversion: Converted item counts to a binary format (1 for purchased, 0 for not purchased).
Market Basket Analysis:

Frequent Itemsets: Applied the Apriori algorithm to identify frequent itemsets with a minimum support threshold of 0.05.
Association Rules: Generated association rules from the frequent itemsets, focusing on rules with a confidence threshold of at least 0.3.
Evaluation Metrics: Assessed rules based on lift, confidence, leverage, and conviction.
Results:

The analysis identified strong associations between various items, such as:
WOODLAND CHARLOTTE BAG and RED RETROSPOT CHARLOTTE BAG: High lift and confidence values indicate a strong relationship.
PLASTERS IN TIN WOODLAND ANIMALS and PLASTERS IN TIN CIRCUS PARADE: Frequently purchased together with high confidence.
Visualized the top association rules, highlighting items often bought together.
This analysis provides insights into customer purchasing patterns, helping businesses optimize inventory management, cross-selling strategies, and marketing campaigns.
