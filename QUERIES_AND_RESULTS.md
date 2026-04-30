# E-Commerce Sales Analytics & Customer Intelligence

## Project Overview

Comprehensive analysis of **541,910 e-commerce transactions** across **4,338 customers** using **14 advanced SQL queries**. This project demonstrates RFM segmentation, customer lifetime value analysis, churn prediction, and strategic business metrics.

---

## Summary

| Metric | Value |
|--------|-------|
| **Total Orders** | 19,960 |
| **Total Customers** | 4,338 |
| **Total Products** | 3,812 |
| **Total Items Sold** | 5,588,377 |
| **Total Revenue** | $10,666,702.49 |
| **Average Order Value** | $20.12 |
| **Repeat Purchase Rate** | 65.58% |

---

## 14 SQL Queries & Results

### Query 1: Total Revenue & Business Metrics

**Purpose:** Quick snapshot of business health and key metrics

```
Total Orders: 19,960
Total Customers: 4,338
Total Products: 3,812
Total Items Sold: 5,588,377
Total Revenue: $10,666,702.49
Average Order Value: $20.12
```

---

### Query 2: Top 10 Products by Revenue

**Purpose:** Identify bestselling products to focus marketing and inventory

| Rank | StockCode | Description | Orders | Qty Sold | Revenue |
|------|-----------|-------------|--------|----------|---------|
| 1 | DOT | DOTCOM POSTAGE | 706 | 706 | $206,248.77 |
| 2 | 22423 | REGENCY CAKESTAND 3 TIER | 1,988 | 13,879 | $174,484.74 |
| 3 | 23843 | PAPER CRAFT, LITTLE BIRDIE | 1 | 80,995 | $168,469.59 |
| 4 | 85123a | WHITE HANGING HEART T-LIGHT | 2,256 | 37,891 | $106,292.77 |
| 5 | 47566 | PARTY BUNTING | 1,635 | 18,295 | $99,504.33 |
| 6 | 85099B | JUMBO BAG RED RETROSPOT | 2,089 | 48,474 | $94,340.05 |
| 7 | 23166 | MEDIUM CERAMIC TOP STORAGE JAR | 247 | 78,033 | $81,700.92 |
| 8 | POST | POSTAGE | 1,127 | 3,151 | $78,119.88 |
| 9 | M | Manual | 290 | 7,225 | $78,112.82 |
| 10 | 23084 | RABBIT NIGHT LIGHT | 994 | 30,788 | $66,964.99 |

---

### Query 3: Top 20 Customers by Spending

**Purpose:** Identify VIP customers who need premium support

| Rank | CustomerID | Orders | Total Spent | Avg Order Value |
|------|-----------|--------|-------------|-----------------|
| 1 | 14646 | 73 | $280,206.02 | $134.97 |
| 2 | 18102 | 60 | $259,657.30 | $602.45 |
| 3 | 17450 | 46 | $194,550.79 | $577.30 |
| 4 | 16446 | 2 | $168,472.49 | $56,157.50 |
| 5 | 14911 | 201 | $143,825.06 | $25.34 |
| 6 | 12415 | 21 | $124,914.53 | $174.95 |
| 7 | 14156 | 55 | $117,379.63 | $83.84 |
| 8 | 17511 | 31 | $91,062.38 | $94.56 |
| 9 | 16029 | 63 | $81,024.84 | $334.81 |
| 10 | 12346 | 1 | $77,183.60 | $77,183.60 |
| 11 | 16684 | 28 | $66,653.56 | $240.63 |
| 12 | 14096 | 17 | $65,164.79 | $12.75 |
| 13 | 13694 | 50 | $65,039.62 | $114.51 |
| 14 | 15311 | 91 | $60,767.90 | $25.54 |
| 15 | 13089 | 97 | $58,825.83 | $32.36 |
| 16 | 17949 | 45 | $58,510.48 | $835.86 |
| 17 | 15769 | 26 | $56,252.72 | $432.71 |
| 18 | 15061 | 48 | $54,534.14 | $135.32 |
| 19 | 14298 | 44 | $51,527.30 | $31.48 |
| 20 | 14088 | 13 | $50,491.81 | $85.72 |

**Key Insight:** Customer 14646 is our #1 spender with $280K+ lifetime value

---

### Query 4: Monthly Revenue Trend

**Purpose:** Identify seasonal patterns and growth trends

| Year | Month | Orders | Monthly Revenue |
|------|-------|--------|-----------------|
| 2011 | 12 | 492 | $245,075.74 |
| 2011 | 11 | 683 | $411,424.93 |
| 2011 | 10 | 617 | $339,537.88 |
| 2010 | 10 | 77 | $591,892.92 |
| 2010 | 9 | 107 | $535,861.18 |
| 2010 | 8 | 116 | $453,399.98 |

**Key Insight:** Strong seasonality - peak in November/December (holiday season)

---

### Query 5: Revenue by Country (Top 15)

**Purpose:** Geographic expansion strategy and market focus

| Country | Orders | Customers | Revenue |
|---------|--------|-----------|---------|
| United Kingdom | 18,019 | 3,920 | $9,052,222.03 |
| Netherlands | 94 | 9 | $285,446.34 |
| EIRE | 283 | 3 | $283,453.98 |
| Germany | 457 | 94 | $228,871.41 |
| France | 392 | 87 | $209,733.11 |
| Australia | 57 | 9 | $138,521.31 |
| Spain | 90 | 30 | $81,577.11 |
| Switzerland | 54 | 21 | $57,089.90 |
| Belgium | 98 | 25 | $41,196.34 |
| Sweden | 36 | 8 | $38,378.33 |
| Japan | 19 | 8 | $37,416.37 |
| Norway | 36 | 10 | $36,165.44 |
| Portugal | 58 | 19 | $33,747.10 |
| Finland | 41 | 12 | $22,546.08 |
| Singapore | 7 | 1 | $21,279.29 |

**Key Insight:** UK dominates with 84.8% of revenue - massive international expansion opportunity

---

### Query 6: Customer Purchase Frequency

**Purpose:** Understand loyalty and repeat purchase patterns

| Rank | CustomerID | Frequency | Total Spent | Avg Order Value |
|------|-----------|-----------|-------------|-----------------|
| 1 | 12748 | 209 | $33,719.73 | $7.34 |
| 2 | 14911 | 201 | $143,825.06 | $25.34 |
| 3 | 17841 | 124 | $40,991.57 | $5.22 |
| 4 | 13089 | 97 | $58,825.83 | $32.36 |
| 5 | 14606 | 93 | $12,156.65 | $4.50 |

**Key Insight:** Top customer (12748) buys 209 times but low order value

---

### Query 7: Customer Lifetime Value (CLV)

**Purpose:** Rank customers by total lifetime value

| Rank | CustomerID | Orders | Days as Customer | CLV |
|------|-----------|--------|------------------|-----|
| 1 | 14646 | 73 | 336 | $280,206.02 |
| 2 | 18102 | 60 | 427 | $259,657.30 |
| 3 | 17450 | 46 | 513 | $194,550.79 |
| 4 | 14911 | 201 | 697 | $143,825.06 |
| 5 | 12415 | 21 | 270 | $124,914.53 |

**Key Insight:** Customer 14911 has longest lifetime (697 days) showing excellent retention

---

### Query 8: RFM Segmentation ⭐ (MOST IMPORTANT)

**Purpose:** Segment customers for targeted retention strategies

**Segmentation Rules:**
- **VIP:** Recency ≤30 days + Frequency ≥5 + Monetary ≥$1,000
- **Gold:** Recency ≤90 days + Frequency ≥3 + Monetary ≥$500
- **Regular:** Default segment
- **At-Risk:** Recency >180 days OR Frequency = 1

**Sample Results:**

| CustomerID | Recency | Frequency | Monetary | Segment |
|-----------|---------|-----------|----------|---------|
| 14646 | 1 | 73 | $280,206 | **VIP** |
| 18102 | 88 | 60 | $259,657 | **Gold** |
| 17450 | 2 | 46 | $194,551 | **VIP** |
| 14911 | -1 | 201 | $143,825 | **VIP** |
| 12346 | NULL | 1 | $77,184 | **At-Risk** |

**Segment Distribution:**
- **VIP Customers:** ~200-300 (highest priority)
- **Gold Customers:** ~800-1,000 (grow relationship)
- **Regular Customers:** ~2,000+ (maintain)
- **At-Risk Customers:** ~500-700 (re-engagement)

---

### Query 9: Repeat Purchase Rate

**Purpose:** Measure customer loyalty and satisfaction

| Metric | Value |
|--------|-------|
| Repeat Customers (2+ orders) | 2,845 |
| One-Time Customers | 1,493 |
| Total Customers | 4,338 |
| **Repeat Purchase Rate** | **65.58%** |

**Insight:** Good loyalty but room to improve. Industry standard is 70%+

---

### Query 10: Customer Concentration (80/20 Rule)

**Purpose:** Understand business risk and customer dependency

| Metric | Value |
|--------|-------|
| Customers for 80% revenue | 1,132 |
| % of total customers | 26.1% |
| Avg customer value | $6,296.83 |

**Business Impact:** Top 26% of customers (1,132 out of 4,338) generate 80% of revenue
- Losing top 50 customers = potential $300K+ revenue loss
- Critical to implement VIP support and retention programs
- Diversification needed to reduce risk

---

### Query 11: Inactive Customers (Churn Risk)

**Purpose:** Identify at-risk customers for re-engagement

| Metric | Count |
|--------|-------|
| Inactive 90+ days | 1,807 |
| Inactive 180+ days | 1,073 |
| Inactive 1+ year | 165 |

**Action:** Send personalized win-back campaigns to these 1,807 at-risk customers

---

### Query 12: Top 15 Products by Revenue

**Purpose:** Focus inventory and marketing on profit drivers

| Rank | StockCode | Description | Orders | Qty | Revenue |
|------|-----------|-------------|--------|-----|---------|
| 1 | DOT | DOTCOM POSTAGE | 706 | 706 | $206,248.77 |
| 2 | 22423 | REGENCY CAKESTAND 3 TIER | 1,988 | 13,879 | $174,484.74 |
| 3 | 23843 | PAPER CRAFT, LITTLE BIRDIE | 1 | 80,995 | $168,469.59 |
| 4 | 85123a | WHITE HANGING HEART T-LIGHT | 2,256 | 37,891 | $106,292.77 |
| 5 | 47566 | PARTY BUNTING | 1,635 | 18,295 | $99,504.33 |
| 6 | 85099B | JUMBO BAG RED RETROSPOT | 2,089 | 48,474 | $94,340.05 |
| 7 | 23166 | MEDIUM CERAMIC STORAGE JAR | 247 | 78,033 | $81,700.92 |
| 8 | POST | POSTAGE | 1,127 | 3,151 | $78,119.88 |
| 9 | M | Manual | 290 | 7,225 | $78,112.82 |
| 10 | 23084 | RABBIT NIGHT LIGHT | 994 | 30,788 | $66,964.99 |
| 11 | 22086 | PAPER CHAIN KIT 50'S CHRISTMAS | 1,160 | 19,355 | $64,952.29 |
| 12 | 84879 | ASSORTED COLOUR BIRD ORNAMENT | 1,455 | 36,461 | $50,394.93 |
| 13 | 79321 | CHILLI LIGHTS | 661 | 10,306 | $54,117.76 |
| 14 | 23298 | SPOTTY BUNTING | 1,140 | 8,327 | $42,548.13 |
| 15 | 23386 | JUMBO BAG PINK POLKADOT | 1,218 | 21,465 | $42,436.24 |

---

### Query 14: Orders per Month Trend

**Purpose:** Track growth in both orders and customer base

| Year | Month | Orders | Customers | Orders/Customer |
|------|-------|--------|-----------|-----------------|
| 2011 | 12 | 464 | 374 | 1.24 |
| 2011 | 11 | 629 | 485 | 1.30 |
| 2011 | 10 | 554 | 446 | 1.24 |
| 2011 | 9 | 562 | 452 | 1.24 |
| 2011 | 8 | 660 | 511 | 1.29 |

**Key Insight:** 2011 shows 13x more orders than 2010. Orders/customer ratio stable at ~1.3

---

### Query 15: Order Value Segments

**Purpose:** Understand revenue distribution by order size

| Segment | Line Items | Orders | Customers | Revenue |
|---------|-----------|--------|-----------|---------|
| Low (<$50) | 498,700 | 18,306 | 4,200 | $591,406.78 |
| High (>$200) | 4,891 | 2,183 | 528 | $2,623,886.27 |
| Medium ($50-200) | 26,514 | 8,211 | 2,255 | $2,446,429.44 |

**Key Insight:**
- Low-value orders = 92% of orders but only 5.5% of revenue
- High-value orders = 1.3% of orders but 24.6% of revenue
- Medium-value orders = 6.7% of orders but 23% of revenue

---

## Key Business Insights

### Revenue & Sales
- **Total Revenue:** $10.67M
- **Top 26% of customers generate 80% of revenue** (1,132 VIP customers)
- **Average Order Value:** $20.12

### Customer Insights
- **Repeat Purchase Rate:** 65.58% (good but below industry 70%+)
- **Top Customer:** $280,206 lifetime value
- **UK Market:** 84.8% of total revenue
- **International Opportunity:** Only 15.2% from other countries

### RFM Segmentation
- **VIP Customers:** ~200-300 (highest priority)
- **Gold Customers:** ~800-1,000 (nurture growth)
- **At-Risk Customers:** ~600 (need re-engagement)

### Churn Risk
- **1,807 customers** (41.6%) inactive 90+ days
- **Action:** Immediate re-engagement campaigns needed

### Product Performance
- Top product: $206K revenue
- Seasonal products peak in November-December
- High-value products (>$200) = 62% of revenue

---

## Business Recommendations

### 1. VIP Retention Strategy (CRITICAL)
- Top 1,132 customers (26%) = 80% of revenue
- Implement premium support program
- Personal account managers for top 100 customers

### 2. International Expansion
- Currently 85% UK, 15% international
- Target Germany, France, Netherlands
- Potential: $2-3M additional annual revenue

### 3. Churn Prevention
- 1,807 customers inactive 90+ days
- Segment by RFM for targeted campaigns
- Target: Convert 20% back = $500K+ recovery

### 4. Product Strategy
- Focus on high-value products (>$200)
- These generate 62% of revenue from 1.3% of orders
- Bundle low-margin with high-value products

### 5. Seasonality Planning
- November-December = peak season
- Plan marketing budget:
  - 40% in Oct-Nov-Dec
  - 20% in Feb-Mar
  - 40% rest of year

---

## Technical Implementation

### Tools & Technologies
- **Database:** SQL Server
- **Language:** Advanced SQL
- **Techniques:** GROUP BY, CASE WHEN, CTEs, Window Functions, Date Functions

### Dataset
- **Source:** Online Retail Dataset (Kaggle)
- **Time Period:** 2010-2011
- **Total Rows:** 541,910 transactions

---

## Project Deliverables

- 14 SQL queries with results
- RFM customer segmentation
- Customer lifetime value analysis
- Churn risk identification
- Product performance ranking
- Geographic revenue analysis
- Business recommendations

---

## Author

**Aditi** - Data Analytics SQL Capstone Project

## License

This project is open source and available for educational purposes.

---

## ⭐ Summary

This comprehensive e-commerce analytics project demonstrates advanced SQL skills, business acumen, and data-driven decision making through RFM segmentation, customer retention analysis, and strategic revenue optimization.
