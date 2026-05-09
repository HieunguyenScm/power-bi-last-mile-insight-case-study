# Last-Mile Delivery Performance Analysis

## 1. Project Overview

This project analyzes last-mile delivery performance using Power BI.  
The dataset focuses on delivery assignment, successful delivery rate, payload capacity, HR cost, rider productivity, and operational leakage.

## 2. Business Context

The objective of this case study is to identify operational bottlenecks in the last-mile delivery process and propose actionable recommendations to improve delivery success rate and reduce post-assignment leakage.

## 3. Key Insight

The main issue is not only the number of inbound orders or the assignment rate.  
The assignment rate is already 89.4%, but only 552 out of 650 assigned orders were successfully delivered.

This means there are 98 assigned-but-not-successful orders, showing a leakage in last-mile execution.

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

## 5. Main Findings

### 5.1 Post-assignment leakage is the biggest issue

Although most new orders were assigned, a significant number of assigned orders did not convert into successful deliveries.

### 5.2 Payload is not the only bottleneck

The average assigned payload is around 14.27 kg/order, which does not immediately indicate severe overload. However, heavy orders above 20kg should still be managed separately.

### 5.3 Early execution before 9:30 is important

Orders handled earlier in the day may improve delivery success because the operation team has more time to solve exceptions.

### 5.4 Rider productivity should be optimized

The operation should not only increase headcount but also improve orders per rider, successful deliveries per rider, and error control.

## 6. Recommendations

1. Track assigned-but-not-successful orders separately.
2. Add reason codes for every failed delivery.
3. Increase the percentage of orders delivered before 9:30.
4. Manage heavy orders above 20kg as a separate operational group.
5. Improve rider productivity through route optimization, training, and incentive design.

## 7. Conclusion

The key improvement opportunity is to convert more assigned orders into successful deliveries by reducing post-assignment leakage, improving early-day execution, managing heavy orders separately, and optimizing rider productivity.
