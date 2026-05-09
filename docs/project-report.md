# Supply Chain Operations Performance & Visibility Report

## 1. Executive Summary

This report analyzes a supply chain operations dashboard built in Power BI, focusing on delivery execution, order assignment, payload capacity, HR cost, and rider productivity.

The main objective of this project is to identify operational leakage, improve performance visibility, and propose actionable recommendations to support faster and better decision-making in supply chain operations.

The key insight from the analysis is that the main issue is not only the number of inbound orders or the assignment rate. The assignment rate reached 89.4%, which means most new orders were assigned. However, only 552 out of 650 assigned orders were successfully delivered.

This created 98 assigned-but-not-successful orders, showing a clear leakage after assignment.

Therefore, the biggest improvement opportunity is to improve execution quality after orders have already entered the delivery operation.

---

## 2. Business Context

In supply chain operations, performance issues often come from multiple factors such as manual tracking, low visibility, delayed execution, inefficient allocation, limited capacity planning, and weak root-cause analysis.

A dashboard is valuable because it helps the operation team track key performance indicators, identify bottlenecks, and make faster decisions.

This project focuses on the following business questions:

- How many orders are received, assigned, and successfully delivered?
- Where does operational leakage happen?
- How many assigned orders fail to convert into successful delivery?
- How does payload affect delivery execution?
- How do HR cost and rider productivity relate to delivery performance?
- What actions can improve service level and operational efficiency?

---

## 3. Dataset Overview

The Power BI dashboard uses operational data related to:

- Last-mile delivery performance
- Inbound and assignment performance
- Payload capacity
- HR cost and rider income
- Successful deliveries
- Failed orders
- Heavy orders
- Delivery productivity

The dataset supports analysis across four major operational dimensions:

1. Order flow performance
2. Delivery success performance
3. Payload and capacity performance
4. HR cost and rider productivity performance

---

## 4. Key Metrics

| Metric | Value |
|---|---:|
| New Orders | 725 |
| Assigned Orders | 650 |
| Successful Deliveries | 552 |
| Assignment Rate | 89.4% |
| GTC on New Orders | 76.21% |
| GTC on Assigned Orders | 84.96% |
| Assigned-but-not-GTC Orders | 98 |
| Assigned Payload | 9,277 kg |
| Average Payload per Assigned Order | 14.27 kg/order |

---

## 5. Order Funnel Analysis

The delivery process can be viewed as an operational funnel:

| Stage | Orders | Conversion |
|---|---:|---:|
| New Orders | 725 | 100% |
| Assigned Orders | 650 | 89.4% |
| Successful Deliveries | 552 | 76.21% |

From this funnel, there are two major leakage points.

### 5.1 Unassigned Orders

There were 725 new orders, but only 650 were assigned.

Unassigned orders:

725 - 650 = 75 orders

This means 75 orders did not enter the delivery assignment process.

Possible causes include:

- Late order arrival
- Limited delivery capacity
- Lack of available riders
- Data or system issues
- Orders not ready for delivery
- Cut-off time issues

### 5.2 Assigned-but-not-Successful Orders

There were 650 assigned orders, but only 552 were successfully delivered.

Assigned-but-not-successful orders:

650 - 552 = 98 orders

This is the most important issue because these orders already consumed operational resources but did not generate successful delivery outcomes.

These resources may include:

- Rider capacity
- Vehicle usage
- Handling time
- Route planning effort
- Delivery cost
- Management attention

This shows that the main improvement opportunity is not only assigning more orders, but converting more assigned orders into successful deliveries.

---

## 6. Key Insight: Post-Assignment Leakage

The biggest insight from the dashboard is post-assignment leakage.

Although the assignment rate was relatively high at 89.4%, the successful delivery rate on assigned orders was only 84.96%.

This means the operation can assign orders, but still loses performance during execution.

In business terms, the operation has a conversion problem after assignment.

This is important because assigned-but-not-successful orders are more costly than unassigned orders. An unassigned order may indicate a planning or capacity issue, but an assigned failed order means the business has already spent resources without achieving the final service outcome.

Therefore, the key KPI that should be tracked is:

Assigned-but-not-GTC Orders = Assigned Orders - Successful Deliveries

For this case:

650 - 552 = 98 orders

This KPI should be monitored daily to identify where and why delivery failures happen.

---

## 7. Payload Capacity Analysis

The assigned payload was 9,277 kg across 650 assigned orders.

Average payload per assigned order:

9,277 / 650 = 14.27 kg/order

At the overall level, this does not immediately indicate severe overload. However, average payload can hide operational pressure from heavy orders.

Heavy orders may affect delivery execution because they can:

- Increase loading and unloading time
- Require more suitable vehicles
- Reduce the number of orders per trip
- Increase rider fatigue
- Increase route completion time
- Require different incentive or compensation logic

Therefore, heavy orders should be monitored separately, especially orders above 20kg.

Recommended payload KPIs:

- Average kg per order
- Heavy order rate
- GTC rate for heavy orders
- Cost per heavy order
- Heavy orders per trip
- Heavy orders per rider

---

## 8. HR Cost and Rider Productivity Analysis

The dashboard also connects delivery performance with HR cost and rider productivity.

This is important because improving supply chain performance is not only about increasing headcount or adding more vehicles. The operation must understand whether its current resources are being used efficiently.

Important productivity KPIs include:

- Orders per rider
- Successful deliveries per rider
- Failed orders per rider
- Cost per order
- Incentive per successful delivery
- Penalty per failed order
- Heavy orders handled per rider

If the operation increases headcount but successful deliveries do not improve proportionally, the business may face higher cost without better service performance.

Therefore, the operation should focus on improving productivity, not only capacity.

---

## 9. Root Cause Hypotheses

Based on the dashboard, the assigned-but-not-successful orders may come from several root causes.

### 9.1 Customer-related issues

Possible issues:

- Customer not available
- Customer reschedules delivery
- Wrong phone number
- Wrong address
- Customer refuses delivery

### 9.2 Rider-related issues

Possible issues:

- Rider cannot complete the route on time
- Rider receives too many orders
- Rider is unfamiliar with the area
- Rider lacks experience
- Rider avoids heavy or difficult orders

### 9.3 Route and capacity issues

Possible issues:

- Route is too long
- Orders are not grouped efficiently
- Heavy orders are not planned separately
- Vehicle capacity is not suitable
- Too many orders are assigned late in the day

### 9.4 Warehouse or process issues

Possible issues:

- Picking delay
- Sorting delay
- Loading delay
- Incorrect order preparation
- Order not ready before dispatch

### 9.5 System and data issues

Possible issues:

- Incorrect order status
- Missing reason codes
- Data not updated on time
- Lack of visibility on failed delivery reasons

---

## 10. Recommendations

### 10.1 Track Assigned-but-not-GTC as a separate KPI

The operation should not only track successful deliveries. It should separately track assigned orders that fail to become successful deliveries.

Recommended KPI:

Assigned-but-not-GTC Rate = Assigned-but-not-GTC Orders / Assigned Orders

For this case:

98 / 650 = 15.08%

This metric shows the quality of execution after assignment.

---

### 10.2 Add failure reason codes

Every unsuccessful delivery should have a clear reason code.

Suggested reason codes:

- Customer not available
- Wrong address
- Customer rescheduled
- Late delivery
- Heavy order issue
- Vehicle capacity issue
- Rider issue
- Warehouse delay
- System/data issue
- Cancelled order
- Pending status

This will help the team move from “knowing what happened” to “knowing why it happened.”

---

### 10.3 Improve early-day execution

The team should improve early execution to reduce end-of-day pressure.

Recommended actions:

- Prepare orders before dispatch time
- Sort orders by route earlier
- Prioritize far routes and heavy orders
- Confirm difficult orders with customers earlier
- Monitor orders not dispatched before a defined cut-off time

Early execution gives the team more time to solve exceptions and reattempt failed deliveries.

---

### 10.4 Monitor heavy orders separately

Orders above 20kg should be treated as a specific operational group.

Recommended actions:

- Create a separate heavy-order dashboard
- Monitor GTC rate for heavy orders
- Assign heavy orders to suitable riders or vehicles
- Design proper incentive for heavy-order handling
- Group heavy orders by route to improve load planning

---

### 10.5 Improve rider productivity

The operation should focus on improving productivity per rider.

Recommended actions:

- Track orders per rider
- Track successful deliveries per rider
- Track failed orders per rider
- Compare productivity between experienced and new riders
- Provide training for new riders
- Allocate difficult routes to more experienced riders
- Align incentives with successful delivery quality

---

### 10.6 Use dashboard insights for faster decision-making

The dashboard should be used as a daily decision-support tool.

Recommended dashboard views:

- Daily order funnel
- Assigned-but-not-GTC tracking
- Error reason analysis
- Payload and heavy order view
- Rider productivity view
- Cost per order view
- Early execution tracking

This helps the team identify problems earlier and take action faster.

---

## 11. Relevance to Supply Chain Internship Role

This project is relevant to supply chain roles that require data-driven tools, digital solutions, process improvement, and operational decision support.

The project demonstrates the ability to:

- Build a Power BI dashboard for supply chain performance tracking
- Use Power Query to clean and transform operational data
- Create KPI views for business visibility
- Analyze operational leakage
- Identify root causes behind performance issues
- Translate data insights into practical recommendations
- Support decision-making through dashboard design
- Connect supply chain operations with cost and productivity

These skills are relevant to supply chain internship roles involving planning support, stock allocation, automation, digital tools, and cross-functional collaboration.

---

## 12. Conclusion

The key improvement opportunity is to convert more assigned orders into successful deliveries.

The dashboard shows that the assignment rate is relatively strong, but delivery execution after assignment still has leakage.

With 650 assigned orders and 552 successful deliveries, there are 98 assigned-but-not-successful orders. This represents an execution gap that should be investigated and improved.

The recommended focus areas are:

1. Track assigned-but-not-GTC orders
2. Add clear failure reason codes
3. Improve early-day execution
4. Monitor heavy orders separately
5. Improve rider productivity
6. Use dashboard visibility for faster operational decisions

This project shows how Power BI can be used as a supply chain decision-support tool to improve visibility, identify operational bottlenecks, and support practical business improvements.
