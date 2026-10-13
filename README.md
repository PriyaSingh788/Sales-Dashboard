# 🎧 boAt Sales Dashboard (Power BI)

An interactive Power BI dashboard analysing sales, profit, customers and channels for a consumer-audio and wearables brand (boAt-style product catalogue). It covers KPIs, customer segmentation, product-category performance, monthly trends, sales-vs-target tracking and order-status analysis.

## 📌 Overview

The report has two main pages:

- **Page 1 – Boat Dashboard:** headline KPIs, customer and product breakdowns, and AI-driven insights.
- **Page 2 – Sales Performance & Operations:** time trends, target tracking, category contribution, profit build-up, order status and channel/tier flow.

## 📊 Page 1 – Boat Dashboard

| Visual | What it shows |
|---|---|
| KPI cards | Max of Profit, Total Sales, Sum of Quantity, Sum of Weekend sales |
| Line chart | Count of CustomerSegment by CustomerTier (Tier-1 to Tier-3) |
| Key Influencers | What drives Profit up, e.g. a drop in DiscountPct |
| Donut chart | Sum of NetSales by CustomerSegment (Young Professional, Student, Working Professional, Family Buyer, Gamer, Gift Buyer) |
| Pie chart | Count of ProductID by ProductCategory |
| Bar chart | Sum of SellingPrice by Quantity |
| Scatter plot | SellingPrice vs Profit (bubble size = Quantity) by ProductCategory |

## 📈 Page 2 – Sales Performance & Operations

| Visual | What it shows |
|---|---|
| Area/column chart | Sum of Total Net-Sales by Month |
| Gauge | Total Net-Sales against Sales Target |
| Treemap | Net-Sales share by ProductCategory (True Wireless Earbuds, Neckbands, Smart Watches, Wireless Speakers, Headphones, etc.) |
| Waterfall chart | Cumulative Profit contribution by ProductCategory |
| Funnel | Count of SalesID by OrderStatus (Delivered, Returned, Cancelled) |
| Decomposition / flow visual | Net-Sales broken down by ChannelType (Online/Offline) and CustomerTier |

## 🛠️ Tools & Features Used

- **Power BI Desktop**
- **Data modeling** across fact and dimension tables (Sales, Product, Customer, etc.)
- **DAX measures** for Net Sales, Profit, Sales Target, Weekend Sales
- **AI visuals:** Key Influencers, Decomposition Tree
- **Navigation:** back button and page navigation
- Consistent dark-green theme

## 🗂️ Data Model

Key fields used: `SalesID`, `ProductID`, `ProductCategory`, `CustomerSegment`, `CustomerTier`, `ChannelType`, `OrderStatus`, `SellingPrice`, `Quantity`, `DiscountPct`, `NetSales`, `Profit`, `Month`.

> Add your table relationships screenshot here:
> `![Data Model](images/data-model.png)`

## 🔍 Key Insights

- Over 90% of orders are **Delivered**, with a small share Returned (~45K) or Cancelled (~16K).
- **True Wireless Earbuds** is the largest category by both product count and net sales, followed by Neckbands and Smart Watches.
- **Online** is the dominant sales channel compared to Offline.
- Lower discount percentages are associated with higher average profit (Key Influencers).
- Profit contribution is concentrated in the top few product categories.

> Verify these figures against your final data before publishing.

## 🚀 How to Use

1. Clone or download this repository.
2. Open `data modeling.pbix` in **Power BI Desktop**.
3. If prompted, update the data source path under **Transform data → Data source settings**.
4. Click **Refresh** and explore the pages using slicers, tooltips and cross-filtering.

## 📁 Repository Structure

```
├── data modeling.pbix     # Power BI report
├── data/                  # Source dataset(s)
├── images/                # Dashboard screenshots
└── README.md
```

## 🖼️ Screenshots

![Page 1](images/Page 1.png)
![Page 2](images/Page 2.png)

## 👤 Author

**Your Name**
·[GitHub](https://github.com/PriyaSingh788)

---
⭐ If you found this useful, consider starring the repo!
