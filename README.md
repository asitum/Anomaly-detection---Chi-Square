# Anomaly Detection in Transactions

**Author:** Antoni Šitum  
**Service:** CHI-SQUARE - Data Science for Business

## Overview
Anomaly detection using Isolation Forest algorithm to identify suspicious transactions that may indicate fraud, errors, or unusual purchasing patterns.

## Dataset
- Superstore dataset (9,994 transactions)
- Features: Sales, Quantity, Discount, Profit
- Period: 2014-2017

## Methodology
- **Primary method:** Isolation Forest (contamination=0.05)
- **Alternative method:** DBSCAN (eps=1.8, min_samples=5)

## Results

| Metric | Normal | Anomaly | Ratio |
|--------|--------|---------|-------|
| Avg Sales (EUR) | 151 | 1,723 | 11.4x |
| Avg Quantity | 3.6 | 6.6 | 1.8x |
| Avg Discount | 14.8% | 31.2% | 2.1x |
| Avg Profit (EUR) | 22 | 162 | 7.4x |

## Key Findings
- **500 transactions (5%) detected as anomalies**
- Anomalies have 11x higher average sales
- Anomalies have 2x higher average discount
- Isolation Forest outperforms DBSCAN for business-relevant anomalies

## Technologies
- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
- Isolation Forest, DBSCAN

## Contact
Antoni Šitum – chisquare.analiza@gmail.com  
CHI-SQUARE – Data science for businesses
