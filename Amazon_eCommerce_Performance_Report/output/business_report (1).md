# Amazon eCommerce Performance Report: Revenue, Risk & Fulfillment Efficiency

_Date range: **2025-01-01** to **2025-12-02** | Generated: 2026-02-25_

## Executive Summary
- From 2025-01-01 to 2025-12-02, total revenue was 161576.08 USD across 500 orders (AOV 323.15) and 966 units.
- Revenue shows an upward trend per advanced_metrics.trend_slope (0.6804284523478589), with notable volatility between the peak day (2025-08-02: 5540.23) and low day (2025-02-17: 628.06).
- Revenue is fairly balanced across marketplaces (Amazon.com 56297.0; Amazon.co.uk 54181.04; Amazon.de 51098.04) and fulfillment (FBM 82336.24 vs FBA 79239.84).
- Refund rate is 0.046 (23 refunded orders) with refunded revenue 5769.95, representing 0.0357 of total revenue.

## KPI Snapshot
| KPI | Value |
|---|---:|
| Total Revenue | $161,576.08 |
| Total Orders | 500 |
| Total Units | 966 |
| Average Order Value (AOV) | $323.15 |
| Refund Rate | 4.60% |

## Revenue & Structure
![](charts/daily_revenue_trend.png)

- **Trend:** Revenue is trending upward over 2025-01-01 to 2025-12-02 based on advanced_metrics.trend_slope = 0.6804284523478589.
- **Volatility:** Daily revenue ranged from 628.06 (low day 2025-02-17) to 5540.23 (peak day 2025-08-02), indicating meaningful volatility around the average daily revenue of 2692.93.
- **Categories:** Top categories by revenue are Toys (31350.3) and Office Supplies (30715.2); the top 3 categories account for 0.5444 of revenue (advanced_metrics.top3_category_share).
- **SKU/ASIN concentration:** Top 10 products by revenue each contribute under 1000 in revenue (max 935.73), suggesting low SKU concentration among the listed top sellers; concentration across all SKUs is not determinable from provided data.
- **Order structure:** Order count is 500 with AOV 323.15 and 966 units; deeper order-size distribution is not determinable from provided data.

### Revenue by Marketplace
- **Amazon.com**: $56,297.00
- **Amazon.co.uk**: $54,181.04
- **Amazon.de**: $51,098.04

### Revenue by Fulfillment Channel
- **FBM**: $82,336.24
- **FBA**: $79,239.84

### Revenue by Category
- **Toys**: $31,350.30
- **Office Supplies**: $30,715.20
- **Electronics**: $25,900.58
- **Sports**: $25,796.38
- **Home & Kitchen**: $25,038.24
- **Beauty**: $22,775.38

## Marketplace Performance
![](charts/revenue_by_marketplace.png)

- Amazon.com is the leading marketplace by revenue (56297.0), followed closely by Amazon.co.uk (54181.04) and Amazon.de (51098.04).
- AOV is highest on Amazon.com (354.07) versus Amazon.co.uk (311.39) and Amazon.de (305.98).
- Marketplace dependency risk appears moderate because revenue is relatively balanced across the three marketplaces; however, refund concentration by marketplace is not determinable from provided data.

## Fulfillment Efficiency (FBA vs FBM)
![](charts/revenue_by_fulfillment.png)

- Revenue is nearly evenly split between FBM (82336.24) and FBA (79239.84).
- FBM has higher AOV (332.0) than FBA (314.44).
- FBA has a slightly lower refund rate (0.0437) than FBM (0.0484).
- Consider scaling FBA selectively where operationally feasible because it has a lower refund rate (0.0437 vs 0.0484), while monitoring the AOV tradeoff (FBA 314.44 vs FBM 332.0).

## Risk & Refund Exposure
- Refund performance shows a 0.046 refund rate (23 orders) with 5769.95 refunded revenue, representing 0.0357 of total revenue (advanced_metrics.refund_revenue_share).
- Refund-rate risk is concentrated in Beauty (0.0779) and Electronics (0.0658), while Sports shows 0.0 and Toys is comparatively low at 0.0222.
### Data limits
- Refund rate and refunded revenue are not segmented by marketplace in the provided data.
- Refunded revenue by category and by fulfillment channel is not provided, only refund rates.
- SKU-level refund behavior is not provided.

## Strategic Recommendations (Prioritized)
**1. Reduce refunds in Beauty and Electronics via tighter listing accuracy, QA checks, and customer expectation management for these categories.**  
- Rationale: These categories have the highest refund rates (Beauty 0.0779; Electronics 0.0658), indicating concentrated refund risk.
- Metric link: risk.refund_rate_by_category

**2. Shift eligible SKUs toward FBA (or test increased FBA allocation) while tracking margin/AOV impact.**  
- Rationale: FBA shows a lower refund rate (0.0437) than FBM (0.0484), though FBM has higher AOV (332.0 vs 314.44).
- Metric link: risk.refund_rate_by_fulfillment and advanced_metrics.aov_by_fulfillment

**3. Protect and grow revenue in the top categories (Toys, Office Supplies, Electronics) through inventory availability and campaign focus.**  
- Rationale: Top 3 categories contribute 0.5444 of revenue, so maintaining performance here materially impacts overall results.
- Metric link: advanced_metrics.top3_category_share and segmentation.revenue_by_category

**4. Lean into Amazon.com growth initiatives (pricing, ads, assortment) while maintaining presence in Amazon.co.uk and Amazon.de.**  
- Rationale: Amazon.com leads revenue (56297.0) and has the highest AOV (354.07), indicating stronger monetization potential.
- Metric link: segmentation.revenue_by_marketplace and advanced_metrics.aov_by_marketplace

**5. Plan for revenue volatility by aligning inventory and operational capacity around peak demand periods identified in the daily trend.**  
- Rationale: Daily revenue shows large swings between 628.06 (low) and 5540.23 (peak), so operations should be resilient to spikes.
- Metric link: trend_summary.peak_day_revenue and trend_summary.low_day_revenue

## Appendix – Data Context
- Rows: **500**
- Currency: **USD**
- Marketplaces: **Amazon.co.uk, Amazon.com, Amazon.de**
- Fulfillment channels: **FBA, FBM**
- Categories: **Beauty, Electronics, Home & Kitchen, Office Supplies, Sports, Toys**
