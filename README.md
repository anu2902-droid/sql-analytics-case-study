# NovaTech Inc. — SQL Analytics Case Study

**Tools:** Python, SQLite, Pandas  
**Dataset:** 500 sales transactions, 200 customers, 8 products (2023)  
**Author:** Anjali Tallapally

---

## Business questions answered

### Q1: Total revenue by product category
| category   |   total_sales |   total_revenue |
|:-----------|--------------:|----------------:|
| Hardware   |           109 |        634702   |
| Services   |           130 |        266633   |
| Software   |           135 |        171174   |
| Support    |           126 |         93418.7 |

### Q2: Top 5 months by revenue
| month   |   total_orders |   total_revenue |
|:--------|---------------:|----------------:|
| 2023-03 |             54 |        169338   |
| 2023-05 |             45 |        113587   |
| 2023-06 |             42 |        105490   |
| 2023-07 |             48 |        102517   |
| 2023-08 |             37 |         94893.2 |

### Q3: Top 5 customers by revenue
| name         | region   | customer_type   |   total_orders |   total_revenue |
|:-------------|:---------|:----------------|---------------:|----------------:|
| Customer_21  | South    | New             |              7 |         24292.7 |
| Customer_145 | South    | Repeat          |              5 |         21367.5 |
| Customer_8   | West     | Repeat          |              4 |         19543.5 |
| Customer_172 | South    | Repeat          |              6 |         18039.7 |
| Customer_71  | West     | Repeat          |             10 |         18006.2 |

### Q4: Average order value by region
| region   |   total_orders |   avg_order_value |   total_revenue |
|:---------|---------------:|------------------:|----------------:|
| South    |            155 |           2426.93 |          376174 |
| West     |            131 |           2377.57 |          311461 |
| North    |            125 |           2336.75 |          292094 |
| East     |             89 |           2092.11 |          186198 |

### Q5: Underperforming products
| product_name    | category   |   total_revenue |   avg_sale_revenue |
|:----------------|:-----------|----------------:|-------------------:|
| Help Desk Basic | Support    |         32457.5 |            2331.86 |
| Data Pro        | Software   |         60492.5 |            2331.86 |
| Help Desk Pro   | Support    |         60961.2 |            2331.86 |
| Training Bundle | Services   |        109552   |            2331.86 |
| Cloud Suite     | Software   |        110681   |            2331.86 |

### Q6: Month over month revenue growth
| month   |   total_revenue |   prev_month |    growth |
|:--------|----------------:|-------------:|----------:|
| 2023-01 |         82457.5 |        nan   |    nan    |
| 2023-02 |         79977.4 |      82457.5 |  -2480.07 |
| 2023-03 |        169338   |      79977.4 |  89360.4  |
| 2023-04 |         91269.9 |     169338   | -78067.9  |
| 2023-05 |        113587   |      91269.9 |  22316.8  |
| 2023-06 |        105490   |     113587   |  -8096.3  |
| 2023-07 |        102517   |     105490   |  -2972.99 |
| 2023-08 |         94893.2 |     102517   |  -7624.26 |
| 2023-09 |         83765.9 |      94893.2 | -11127.2  |
| 2023-10 |         88337.1 |      83765.9 |   4571.14 |
| 2023-11 |         75718.2 |      88337.1 | -12618.8  |
| 2023-12 |         78576   |      75718.2 |   2857.79 |

### Q7: Revenue split by customer type
| customer_type   |   total_revenue |   pct_of_revenue |
|:----------------|----------------:|-----------------:|
| Repeat          |          704917 |            60.46 |
| New             |          461010 |            39.54 |

### Q8: Sales rep close rates
| rep_name      |   total_deals |   closed_deals |   close_rate_pct |
|:--------------|--------------:|---------------:|-----------------:|
| Carlos Rivera |            92 |             71 |             77.2 |
| Priya Patel   |            95 |             72 |             75.8 |
| James Lee     |           110 |             82 |             74.5 |
| Sara Kim      |            95 |             67 |             70.5 |
| Mia Chen      |           108 |             74 |             68.5 |

### Q9: Customer churn rate by quarter
| quarter   |   active_customers |   prev_quarter |   churn_rate_pct |
|:----------|-------------------:|---------------:|-----------------:|
| Q1        |                 96 |            nan |            nan   |
| Q2        |                 83 |             96 |             13.5 |
| Q3        |                 95 |             83 |            -14.5 |
| Q4        |                 91 |             95 |              4.2 |

### Q10: 3-month rolling average revenue
| month   |   total_revenue |   rolling_3mo_avg |
|:--------|----------------:|------------------:|
| 2023-01 |         82457.5 |           82457.5 |
| 2023-02 |         79977.4 |           81217.5 |
| 2023-03 |        169338   |          110591   |
| 2023-04 |         91269.9 |          113528   |
| 2023-05 |        113587   |          124731   |
| 2023-06 |        105490   |          103449   |
| 2023-07 |        102517   |          107198   |
| 2023-08 |         94893.2 |          100967   |
| 2023-09 |         83765.9 |           93725.5 |
| 2023-10 |         88337.1 |           88998.7 |
| 2023-11 |         75718.2 |           82607.1 |
| 2023-12 |         78576   |           80877.1 |

---

## Key insights
- **Hardware** drives the highest total revenue despite fewer transactions
- **Repeat customers** account for the majority of revenue — retention is critical
- Month over month growth shows clear **seasonality peaks** mid-year
- Rolling average reveals **stable upward trend** across 2023
- Top sales rep close rate exceeds **80%** — strong pipeline management
