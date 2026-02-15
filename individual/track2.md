# Track 2 – How a Recommendation Becomes Reality

## 1) What would be implemented (1–2 sentences)?
Implement a churn “risk + segment” flag in the CRM so the retention team can automatically target customers with the highest churn probability and assign the right offer by segment.

## 2) What is the success metric and baseline churn? What is one metric you would not want to get worse?
Success metric: churn rate reduction (or retention lift) among targeted customers.  
Baseline churn in our dataset is ~26.5% (1,496 churned out of 5,636).  
We would not want ARPU / monthly revenue to decrease due to excessive discounts.

## 3) How would you measure impact and what are two risks or unintended consequences?
Measure impact using an A/B test: targeted churn program vs. control group.  
Risks: discount dependency (customers churn after the offer ends) and margin loss from over-incentivizing customers who would have stayed anyway.
