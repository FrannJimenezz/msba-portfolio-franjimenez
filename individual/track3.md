# Track 3 — Deployment + Real-World Use of Predictions

## 1) Instant or overnight?
Overnight is OK because churn risk doesn’t need second-by-second updates.  
A daily/weekly score is enough for retention teams to take action.

## 2) Schedule + where results are saved?
Run weekly scoring (ex: every Monday).  
Save results in a database table like `churn_scores` and connect it to a dashboard/CRM.

## 3) Software approach (high level)
Use a scheduled Python pipeline (or SQL + Python) that retrains and scores automatically.  
Optionally deploy with an API (FastAPI) if teams need on-demand scoring.

## 4) What would you monitor over time?
Data quality: check for missing IDs and missing key fields (monthly_fee, tenure).  
Input drift: monitor changes in feature distributions (ex: contract mix shifts).  
Outcome: track AUC + real churn rate vs predicted churn rate monthly.
