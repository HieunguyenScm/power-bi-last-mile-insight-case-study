# Supply Chain Operations Performance & Visibility Dashboard

## Project Summary

This project presents a Power BI dashboard designed to analyze supply chain operations performance, with a focus on delivery execution, assignment efficiency, payload capacity, HR cost, and rider productivity.

The objective is to improve operational visibility, identify performance leakage, and support faster data-driven decision-making across supply chain operations.

This project demonstrates practical skills in Power BI, Power Query, data modeling, KPI tracking, and business insight generation.

---

## Business Context

In supply chain operations, performance issues often do not come only from demand volume or available capacity. They can also come from poor visibility, manual tracking, delayed execution, inefficient allocation, and lack of root-cause analysis.

This dashboard was developed to answer the following business questions:

- How many orders are received, assigned, and successfully completed?
- Where does operational leakage happen?
- How much assigned volume fails to convert into successful delivery?
- How does payload affect operational capacity?
- How do HR cost, rider productivity, and delivery performance connect?
- What actions can improve service level and operational efficiency?

---

## Dashboard Preview

Dashboard screenshots will be updated once the Power BI report is accessible again.

The Power BI file is available in this repository for review.

---

## Tools Used

- Power BI
- Power Query
- Data Modeling
- DAX
- Excel / CSV
- Supply Chain Operations Analysis
- KPI Dashboard Design
- Business Problem Solving

---

## Key Metrics

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

## Key Insight

The main issue is not only the number of inbound orders or the assignment rate.

Although the assignment rate reached 89.4%, only 552 out of 650 assigned orders were successfully delivered. This created 98 assigned-but-not-successful orders, showing a clear operational leakage after assignment.

This means the biggest improvement opportunity lies in improving execution quality after orders have already entered the delivery operation.

---

## Analysis Highlights

### 1. Post-assignment leakage

The dashboard shows that many orders were already assigned but did not convert into successful deliveries. These orders consume operational resources such as rider capacity, vehicle usage, handling time, and delivery cost, but do not generate successful delivery outcomes.

### 2. Operational visibility

By connecting assignment, successful delivery, payload, HR cost, and productivity indicators, the dashboard improves visibility across the delivery operation and helps identify where performance issues occur.

### 3. Payload and load planning

The average payload per assigned order is around 14.27 kg. While this does not immediately indicate severe overload, heavy orders should still be monitored separately because they may affect route efficiency, handling time, and vehicle planning.

### 4. Productivity and cost control

The dashboard links delivery performance with HR cost and rider productivity. This helps evaluate whether the operation should improve route planning, rider allocation, training, or incentive design instead of only increasing headcount.

---

## Recommendations

1. Track assigned-but-not-GTC orders as a separate KPI.
2. Add failure reason codes for every unsuccessful delivery.
3. Improve early-day execution to reduce end-of-day delivery failures.
4. Monitor heavy orders separately for better load planning.
5. Connect rider productivity with cost and service-level performance.
6. Use dashboard insights to support faster operational decision-making.

---

## Relevance to Supply Chain Internship Role

This project is relevant to supply chain roles that require data-driven tools, operational visibility, planning support, and cross-functional problem solving.

It demonstrates the ability to:

- Build a Power BI dashboard for supply chain performance tracking.
- Use Power Query to clean and transform operational datasets.
- Analyze service-level and execution performance.
- Identify root causes behind operational leakage.
- Translate data insights into practical business recommendations.
- Support decision-making through KPI visibility and dashboard design.

---

## Repository Structure

```text
supply-chain-operations-visibility-dashboard/
│
├── README.md
├── Supply-Chain-Operations-Dashboard.pbix
│
├── images/
│   └── dashboard-overview.png
│
└── docs/
    └── project-report.md
```
## Data Privacy Note

The raw dataset is not publicly shared due to confidentiality.

This repository is used for portfolio demonstration purposes only. Sensitive or confidential data has been removed or anonymized where applicable.

---

## Detailed Report

A detailed business analysis report is available here:

[Read the full project report](docs/project-report.md)

---

## Conclusion

The key improvement opportunity is to convert more assigned orders into successful deliveries by reducing post-assignment leakage, improving operational visibility, managing payload capacity, and optimizing rider productivity.

This project shows how Power BI can be used as a decision-support tool to improve supply chain operations performance.
