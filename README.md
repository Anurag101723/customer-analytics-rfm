# Customer Analytics — RFM Segmentation and K-Means Clustering

RFM analysis and K-Means clustering on 1,067,371 retail transactions to identify customer segments and quantify revenue recovery opportunities.

---

## Overview

In retail, a small percentage of customers typically generate the majority of revenue. Without proper segmentation, businesses treat all customers the same and miss targeted retention, reactivation, and upsell opportunities.

This project builds a complete customer analytics framework using RFM scoring and K-Means clustering on real e-commerce transaction data. The analysis identifies six actionable customer segments, discovers four VIP whale customers generating 1.7M GBP in revenue, and quantifies a 494,723 GBP revenue recovery opportunity.

---

## Results

| Metric | Value |
|---|---|
| Total transactions analysed | 1,067,371 |
| Unique customers segmented | 5,878 |
| Total revenue analysed | 17,743,429 GBP |
| VIP whale customers identified | 4 customers generating 1.7M GBP |
| Average spend per whale customer | 436,835 GBP |
| Revenue recovery opportunity | 494,723 GBP |
| Champions share of revenue | 74% (1,300 customers) |

---

## RFM Customer Segments

| Segment | Customers | Revenue | Recommended Action |
|---|---|---|---|
| Champions | 1,300 | 12.1M GBP | Reward and retain — highest priority |
| Loyal Customers | 1,134 | 2.6M GBP | Upsell and nurture |
| At Risk | 615 | 1.5M GBP | Win-back campaign within 30 days |
| Potential Loyalists | 863 | 402k GBP | Encourage repeat purchases |
| New Customers | 443 | 394k GBP | Onboarding sequence |
| Lost Customers | 1,523 | 667k GBP | Low priority — reactivation cost too high |

---

## K-Means Clusters

| Cluster | Customers | Avg Spend | Total Revenue |
|---|---|---|---|
| VIP Whales | 4 | 436,835 GBP | 1.7M GBP |
| High Value | 35 | 83,086 GBP | 2.9M GBP |
| Loyal Mid-Tier | 3,841 | 3,009 GBP | 11.6M GBP |
| Inactive | 1,998 | 765 GBP | 1.5M GBP |

---

## Revenue Recovery Opportunity

| Action | Estimated Uplift |
|---|---|
| Retain 20% of At-Risk customers | 309,620 GBP |
| Reactivate 10% of Lost customers | 66,712 GBP |
| Convert 30% of New customers | 118,391 GBP |
| Total potential recovery | 494,723 GBP |

---

## EDA Findings

- United Kingdom accounts for over 90% of revenue
- Revenue spikes consistently in October through December each year (Christmas season)
- Most customers spend below 5,000 GBP — classic long-tail distribution
- Top products are seasonal and decorative items

---

## RFM Scoring Method

RFM assigns each customer a score of 1 to 5 across three dimensions.

| Dimension | Definition | Direction |
|---|---|---|
| Recency | Days since last purchase | Lower days = higher score |
| Frequency | Number of unique invoices | Higher frequency = higher score |
| Monetary | Total amount spent | Higher spend = higher score |

Customers scoring 4 or 5 across all three dimensions are classified as Champions.

---

## Methodology

```
UCI Online Retail Dataset (1,067,371 transactions)

Data Cleaning
Remove nulls, cancelled orders (Invoice starts with C),
negative quantities, zero prices

Exploratory Data Analysis
Revenue by country, monthly trends, top products,
customer revenue distribution

RFM Calculation
Reference date set to one day after last transaction
Recency, Frequency, Monetary per customer

RFM Scoring
pd.qcut into quintiles (1 to 5) per dimension
Segment assignment based on score combinations

K-Means Clustering
StandardScaler on RFM features
Elbow method and Silhouette score to select k=4
Cluster labelling based on mean RFM characteristics

Business Recommendations
Revenue recovery opportunity quantified at 494,723 GBP
```

---

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.12 |
| Segmentation | RFM Analysis |
| Clustering | K-Means (Scikit-learn) |
| Preprocessing | StandardScaler, Pandas, NumPy |
| Visualisation | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## Repository Structure

```
customer-analytics-rfm/
|
|-- customer_analytics.ipynb
|-- online_retail_II.csv
|-- README.md
```

---

## How to Run

```bash
git clone https://github.com/Anurag101723/customer-analytics-rfm.git
cd customer-analytics-rfm
pip install pandas numpy scikit-learn matplotlib seaborn
jupyter notebook customer_analytics.ipynb
```

---

## Author

Anurag Rathore  
anuragakrathore@gmail.com  
linkedin.com/in/anurag1017  
anurag101723.github.io
