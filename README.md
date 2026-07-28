# CloudExify Project 2 — Customer Segmentation Analysis

**CloudExify Data Science Internship 2026 — Month 1, Project 2 (Final)**

## Overview

This project segments TrendLine Apparel's customers into value-based groups using RFM (Recency, Frequency, Monetary) analysis followed by K-Means clustering, so the business can tailor marketing and retention efforts to each group.

## Files in this repository

| File | Description |
|---|---|
| `customer_segmentation.ipynb` | Main Jupyter Notebook — RFM calculation, clustering, and visualizations |
| `customer_transactions.csv` | Customer transaction dataset used for the analysis |
| `segmentation_report.txt` | Auto-generated plain-text summary report |
| Screenshot PNGs | Screenshots of the notebook running with outputs and charts |

## What was done

- Loaded transaction-level data and computed RFM (Recency, Frequency, Monetary) features per customer
- Normalized features using `StandardScaler` so no single metric dominates clustering
- Used the Elbow Method **and** Silhouette Score to choose the optimal number of clusters (K=3)
- Applied K-Means clustering to segment customers into High-Value, Mid-Value, and Low-Value groups
- Built a 3D scatter plot visualizing the segments in RFM space
- Profiled each segment's average Recency, Frequency, and Monetary values
- Wrote a specific marketing recommendation for each segment
- Auto-generated a summary report (`segmentation_report.txt`) from the results

## Key Findings

- **High-Value (14.9%)** — recent, frequent, high-spending customers; priority is retention (VIP treatment, loyalty rewards)
- **Mid-Value (51.0%)** — the largest group, moderate activity; best target for growth campaigns (cross-sell, loyalty programs)
- **Low-Value (34.1%)** — long time since last purchase; likely lapsed rather than naturally low-value, so win-back campaigns are recommended over discounting alone

## Tools Used

Python 3 · Jupyter Notebook · pandas · NumPy · matplotlib · scikit-learn (StandardScaler, KMeans, silhouette_score)

## Author

Hafsa Bukhtiar Chishti — Software Engineering, COMSATS University Islamabad, Sahiwal Campus
