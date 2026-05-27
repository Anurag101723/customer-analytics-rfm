# 🛍️ Customer Analytics — RFM Segmentation & K-Means Clustering

> Customer segmentation using RFM analysis and K-Means clustering on 1M+ retail transactions — identifying £494k revenue recovery opportunity and uncovering 4 VIP whale customers generating £1.7M alone.

![Python](https://img.shields.io/badge/Python-3.12-blue?style=flat&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.4-orange?style=flat&logo=scikit-learn&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat)
![Dataset](https://img.shields.io/badge/Dataset-UCI%20Online%20Retail-20BEFF?style=flat&logo=kaggle&logoColor=white)

---

## 📌 Overview

In retail, **20% of customers typically generate 80% of revenue** — but without proper segmentation, businesses treat all customers the same. This project builds a complete customer analytics framework on 1M+ real e-commerce transactions, combining **RFM analysis** and **K-Means clustering** to identify who your best customers are, who is at risk of leaving, and where the biggest revenue opportunities lie.

---

## 🎯 Key Results

| Metric | Value |
|---|---|
| Total transactions analysed | **1,067,371** |
| Unique customers segmented | **5,878** |
| Total revenue analysed | **£17,743,429** |
| VIP Whale customers identified | **4 customers → £1.7M revenue** |
| Revenue recovery opportunity | **£494,723** |
| Champions driving revenue | **1,300 customers → 74% of revenue** |

---

## 💡 Key Discoveries

**🐳 The Whale Finding:**
- Just **4 customers** spend an average of **£436,835 each**
- These 4 people generate **£1.7M in revenue**
- Losing even one = catastrophic business impact
- Recommendation: assign dedicated account managers immediately

**📊 The 80/20 Rule Proven:**
- **1,300 Champions** (22% of customers) generate **74% of all revenue**
- Protecting this segment is the single highest ROI action the business can take

**📅 Seasonal Pattern:**
- Revenue spikes every **October–December** without exception
- Pre-loading inventory and marketing by September is critical

---

## 👥 Customer Segments (RFM Analysis)

| Segment | Customers | Revenue | Strategy |
|---|---|---|---|
| 🏆 Champions | 1,300 | £12.1M | Reward and retain — top priority |
| 💚 Loyal Customers | 1,134 | £2.6M | Upsell and nurture |
| ⚠️ At Risk | 615 | £1.5M | Win-back campaign within 30 days |
| 🆕 New Customers | 443 | £394k | Onboarding sequence to convert |
| 😴 Lost Customers | 1,523 | £667k | Low priority — reactivation cost too high |
| 🌱 Potential Loyalists | 863 | £402k | Encourage repeat purchases |

---

## 🔮 K-Means Clusters

| Cluster | Customers | Avg Spend | Total Revenue |
|---|---|---|---|
| 👑 VIP Whales | 4 | £436,835 | £1.7M |
| 🏆 High Value | 35 | £83,086 | £2.9M |
| 💚 Loyal Mid-Tier | 3,841 | £3,009 | £11.6M |
| 😴 Inactive | 1,998 | £765 | £1.5M |

---

## 💰 Revenue Recovery Opportunity

| Action | Opportunity |
|---|---|
| Retain 20% of At-Risk customers | +£309,620 |
| Reactivate 10% of Lost customers | +£66,712 |
| Convert 30% of New customers | +£118,391 |
| **Total potential recovery** | **~£494,723** |

---

## 🛠️ Tech Stack

- **Language:** Python 3.12
- **Segmentation:** RFM Analysis (Recency, Frequency, Monetary)
- **Clustering:** K-Means (Elbow Method + Silhouette Score)
- **Data Processing:** Pandas, NumPy
- **Scaling:** StandardScaler
- **Visualisation:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

---

## 🔍 Methodology

```
UCI Online Retail Dataset (1,067,371 transactions)
                ↓
Data Cleaning
(remove nulls, cancellations, negative quantities)
                ↓
Exploratory Data Analysis
(revenue by country, monthly trends, top products)
                ↓
RFM Analysis
(Recency, Frequency, Monetary scoring 1-5)
                ↓
RFM Segmentation
(Champions, Loyal, At Risk, Lost, New, Potential)
                ↓
K-Means Clustering
(Elbow Method + Silhouette Score → k=4)
                ↓
Business Recommendations
(£494k revenue recovery opportunity identified)
```

---

## 📁 Repository Structure

```
customer-analytics-rfm/
│
├── customer_analytics.ipynb          # Main analysis notebook
├── online_retail_II.csv              # Dataset
├── README.md                         # Project documentation
```

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/Anurag101723/customer-analytics-rfm.git
cd customer-analytics-rfm
```

2. Install dependencies
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

3. Open the notebook
```bash
jupyter notebook customer_analytics.ipynb
```

---

## 👤 Author

**Anurag Rathore**
M.Sc. Big Data & Business Analytics — FOM University of Applied Sciences
📧 anuragakrathore@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/anurag1017) · [Portfolio](https://Anurag101723.github.io)
