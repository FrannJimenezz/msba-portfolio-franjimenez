# msba-portfolio-franjimenez
MSBA Portfolio Projects and More

# Predictive Analytics Case Competition (Telco Customer Churn)

## Overview
This project analyzes customer churn behavior using a predictive analytics workflow to identify churn drivers, score churn risk, and segment customers for targeted retention strategies. The work was completed as part of a graduate-level case competition in predictive analytics.

## Key Outcomes
- Developed a churn prediction model to estimate customer-level churn probability and support retention prioritization.
- Created customer segments using clustering to support differentiated business recommendations and trade-off analysis.
- Generated a scored holdout dataset for final evaluation and decision-making.

## Repository Structure
- `case-competition-predictive-analytics/Preprocess_Retentiondata.ipynb`  
  Data cleaning and preprocessing workflow.
- `case-competition-predictive-analytics/Final CatBoost Model with Holdout Set Scoring.ipynb`  
  Model training, evaluation, and holdout scoring.
- `case-competition-predictive-analytics/ClusteringKMeans_scaled.ipynb`  
  Customer segmentation using K-Means clustering.
- `case-competition-predictive-analytics/churn_holdout_scored_for_turnin.csv`  
  Final scored holdout output.

## How to Run
1. Clone this repository to your machine.
2. Open Anaconda Navigator and launch Jupyter Notebook.
3. Run `Preprocess_Retentiondata.ipynb` to prepare the dataset.
4. Run `Final CatBoost Model with Holdout Set Scoring.ipynb` to train the model and score churn risk.
5. (Optional) Run `ClusteringKMeans_scaled.ipynb` to reproduce segmentation results.
6. Review the generated output file: `churn_holdout_scored_for_turnin.csv`.

## Limitations / Considerations
This project was completed in a case competition setting using a static dataset. In a real business environment, model performance should be monitored for data drift, and retention strategies should be validated through A/B testing to ensure long-term ROI.

