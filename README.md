# 🛍️ ShopNest Store - Power BI Business Analytics Dashboard

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-FF6F00?style=for-the-badge&logo=microsoft&logoColor=white)](https://docs.microsoft.com/en-us/dax/)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)](https://github.com/yourusername/shopnest-powerbi-analytics)

## 📋 Project Overview

A comprehensive business intelligence solution analyzing Portugal's leading e-commerce platform **ShopNest Store**. This Power BI capstone project delivers actionable insights across sales performance, customer behavior, operational efficiency, and geographic distribution through interactive dashboards and in-depth analytics.

## 🏢 Business Context

**ShopNest Store** serves as Portugal's premier e-commerce department store, connecting small businesses nationwide with customers through a streamlined platform. The company facilitates seamless transactions while providing logistics support for direct customer shipment.

## 📊 Key Performance Indicators

| Metric | Value | Status |
|--------|-------|---------|
| **Total Revenue** | €15.84M | ✅ Strong Performance |
| **Total Orders** | 99K | ✅ High Engagement |
| **Delayed Orders** | 8K (8.1%) | ⚠️ Needs Improvement |
| **Customer Rating** | 4.04/5.0 | ✅ Good Satisfaction |

## 🎯 Project Objectives

- ✅ Analyze comprehensive e-commerce data for actionable insights
- ✅ Answer 8 critical business questions through interactive visualizations
- ✅ Provide strategic recommendations for sales and logistics optimization
- ✅ Demonstrate advanced Power BI and business analytics proficiency

## 📁 Dataset Overview

**Analysis Period:** 2016-2018 | **Total Records:** 1.4M+

| Dataset | Records | Key Information |
|---------|---------|------------------|
| 🛒 Orders | 99,441 | Order lifecycle and delivery tracking |
| 👥 Customers | 99,441 | Geographic and demographic data |
| 📦 Products | 32,951 | Category classification and specifications |
| 💳 Payments | 103,886 | Transaction methods and installments |
| ⭐ Reviews | 99,224 | Customer satisfaction ratings |
| 🏪 Sellers | 3,095 | Merchant network information |
| 🗺️ Geolocation | 1M+ | Geographic coordinate mapping |

## 🔍 Key Analytical Questions Addressed

1. **📈 Category Performance:** Top 10 product categories by revenue
2. **🚚 Logistics Analysis:** Delayed orders by category and timeline
3. **📅 Temporal Trends:** Monthly delivery performance comparison
4. **💰 Payment Insights:** Customer payment method preferences
5. **⭐ Quality Assessment:** Highest and lowest rated categories
6. **🌍 Geographic Distribution:** State-wise sales performance analysis
7. **📊 Seasonal Patterns:** Quarterly sales cycle analysis
8. **📈 Growth Trajectory:** Year-over-year revenue trends

## 📸 Screenshots & Figures  
> **How to use:**  
> 1. Take a screenshot from Power BI.  
> 2. Save it inside `./screenshots/` with the suggested file-name.  
> 3. Commit & push – GitHub will render it automatically.

| # | Section in Report | Placeholder |
|---|-------------------|-------------|
| **1** | Dashboard Overview | `![Dashboard Overview](screenshot/screenshot1.png)` |
| **2** | Top Categories by Total Price | `![Top Categories](screenshot/screenshot2.png)` |
| **3** | Delayed Orders Analysis | `![Delayed Orders](screenshots/delayed_orders.png)` |
| **4** | Monthly Comparison (On-time vs Delayed) | `![Monthly Comparison](screenshots/monthly_on_time_vs_delayed.png)` |
| **5** | Payment Method Analysis | `![Payment Methods](screenshots/payment_methods.png)` |
| **6** | State-wise Sales Map | `![State-wise Sales](screenshots/state_wise_sales.png)` |
| **7** | Product Rating – Highest Rated | `![Highest Rated Categories](screenshots/highest_rated_categories.png)` |
| **8** | Product Rating – Lowest Rated | `![Lowest Rated Categories](screenshots/lowest_rated_categories.png)` |
| **9** | Seasonal Sales Patterns | `![Seasonal Sales Patterns](screenshots/seasonal_sales_patterns.png)` |
| **10** | Revenue Analysis & Yearly Trends | `![Yearly Revenue Trends](screenshots/yearly_revenue_trends.png)` |


## 🏆 Major Findings & Insights

### 🎯 Top Performers
- **Leading Category:** Health & Beauty (€1.26M - 8% of total revenue)
- **Payment Preference:** Credit Cards (74% of transactions)
- **Geographic Leader:** São Paulo State (€3.7M - 23% of revenue)
- **Peak Season:** Q2 represents optimal performance period

### ⚠️ Areas for Improvement
- **Quality Concerns:** Security & Services (2.50/5.0 rating)
- **Logistics Challenges:** Bed, Bath & Table (920 monthly delays)
- **Seasonal Decline:** 39% drop from Q2 to Q4 performance
- **Geographic Gap:** Limited presence in northern/northeastern regions

## 🛠️ Technical Implementation

### Technologies Used
- **Primary Platform:** Microsoft Power BI Desktop
- **Query Language:** DAX (Data Analysis Expressions)
- **Data Architecture:** Star Schema Design
- **Visualization:** Interactive dashboards with cross-filtering

### Key DAX Measures
```dax
// Sales Performance
Total Sales = SUMX(Order_Items, Order_Items[price] + Order_Items[freight_value])
Average Order Value = DIVIDE([Total Sales], [Total Orders])

// Delivery Performance
Delayed Orders = CALCULATE(COUNTROWS(Orders), 
    Orders[order_delivered_customer_date] &gt; Orders[order_estimated_delivery_date])
On-Time Delivery Rate = DIVIDE([Total Orders] - [Delayed Orders], [Total Orders])

// Customer Satisfaction
Average Rating = AVERAGE(Order_Reviews[review_score])
Customer Satisfaction Rate = DIVIDE(
    CALCULATE(COUNT(Order_Reviews[review_score]), Order_Reviews[review_score] &gt;= 4),
    COUNT(Order_Reviews[review_score]))
```

## 📱 Dashboard Features

- **🎛️ Interactive KPI Cards:** Real-time performance monitoring
- **🗺️ Geographic Heat Map:** State-wise sales distribution
- **📊 Category Analysis:** Top performing product segments
- **📈 Trend Analysis:** Temporal patterns and seasonality
- **🔍 Cross-Filtering:** Dynamic data exploration
- **📱 Responsive Design:** Multi-device compatibility

## 💡 Strategic Recommendations

### Immediate Actions (0-3 months)
- 🚨 Emergency quality improvement for Security & Services
- 📦 Specialized logistics for Bed, Bath & Table category
- 📉 Q4 sales recovery strategy implementation

### Medium-term Initiatives (3-12 months)
- 🌍 Geographic expansion to underserved regions
- 💰 Payment method optimization and innovation
- 📊 Category-specific service enhancements

### Long-term Vision (1+ years)
- 🏗️ Infrastructure scaling for continued growth
- 🤖 AI-powered demand forecasting implementation
- 🌱 Sustainable logistics solutions

## 📈 Expected Business Impact

| Initiative | Investment | Expected ROI | Timeline |
|------------|------------|--------------|----------|
| Logistics Optimization | €500K | 15% delay reduction | 6 months |
| Geographic Expansion | €2M | 20% revenue increase | 18 months |
| Category Enhancement | €1M | 12% margin improvement | 12 months |

## 🚀 How to Use This Project

1. **Download:** Clone this repository to your local machine
2. **Open:** Launch the `.pbix` file in Power BI Desktop
3. **Explore:** Use interactive features to explore different insights
4. **Customize:** Modify visualizations based on your requirements
5. **Share:** Publish to Power BI Service for team collaboration

## 📁 Repository Structure

```
📦 shopnest-powerbi-analytics/
├── 📊 ShopNest-Dashboard.pbix          # Main Power BI file
├── 📈 ShopNest-Report.pdf              # Comprehensive analysis report
├── 📋 data/                            # Raw datasets (anonymized)
├── 🖼️ screenshots/                     # Dashboard screenshots
├── 📝 README.md                        # Project documentation
└── 📄 LICENSE                          # MIT License
```

## 🎓 Skills Demonstrated

- **Business Intelligence:** Advanced dashboard development and data modeling
- **Data Analysis:** Statistical analysis and pattern recognition
- **DAX Programming:** Complex measures and calculated columns
- **Data Visualization:** Interactive charts and geographical mapping
- **Business Strategy:** Actionable insights and recommendations
- **Technical Documentation:** Comprehensive reporting and presentation

## 🏆 Achievements

- ✅ Comprehensive analysis of 1.4M+ e-commerce records
- ✅ Identification of €2M+ revenue optimization opportunities
- ✅ Development of data-driven strategic roadmap
- ✅ Creation of interactive business intelligence solution

## 📞 Contact Information

**Deepak Lokhande**
- 📧 Email: your.email@example.com
- 💼 LinkedIn: [linkedin.com/in/deepaklokhande](https://linkedin.com/in/deepaklokhande)
- 🐙 GitHub: [@yourusername](https://github.com/yourusername)
