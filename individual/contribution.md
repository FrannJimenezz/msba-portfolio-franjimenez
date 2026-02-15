# Individual Contribution – Predictive Analytics Case Competition (Churn)

This case competition focused on predicting customer churn and translating the model insights into clear, business-ready recommendations. My individual contribution emphasized building and validating predictive models, interpreting results, and supporting the final segmentation strategy with actionable recommendations and tradeoff framing.

---

## 1) What did I personally contribute to the most?

My strongest contribution was in the **modeling and evaluation portion** of the project, including:

- Building multiple predictive churn models to compare performance and stability:
  - Logistic Regression baseline (numeric dataset)
  - Random Forest (interpretable + strong baseline)
  - Boosting approach (XGBoost-style concept)
  - CatBoost (final high-performing model)

- Designing a **business-driven feature approach**, focusing on variables that are realistic for marketing, retention, and customer success teams to act on.

- Supporting the team’s final workflow by ensuring:
  - The target variable was correctly encoded
  - Models were evaluated consistently using ROC-AUC
  - Results were validated with train/test splits and stability checks

- Helping translate model findings into retention strategy logic:
  - Who is high risk?
  - Why are they leaving?
  - What can the business do differently by segment?

---

## 2) What is one decision or approach I personally advocated for and why?

One approach I strongly advocated for was to treat the project as **more than a “model accuracy” competition** and instead focus on:

### **Model + Interpretability + Actionability**
Rather than using every feature available, I pushed for using models and predictors that:

- Maintain strong performance (ROC-AUC)
- Are explainable to business stakeholders
- Can be directly connected to retention actions (contract conversion, autopay, offers, add-ons)

This helped ensure the final deliverable could be used in a real organization, not just as a technical exercise.

---

## 3) Lessons learned + what I would improve with more time

### **Lesson 1: Strong models still need business framing**
Even with high ROC-AUC performance, the project only becomes valuable when the insights are translated into:
- customer segments,
- retention levers,
- and measurable KPIs.

This reinforced that predictive analytics must always connect back to decision-making.

### **Lesson 2: Retention strategies require tradeoff thinking**
I learned how important it is to communicate tradeoffs clearly. For example:
- Segment 1 retention strategies risk diminishing returns because many customers are already loyal.
- Segment 2 win-back campaigns can be expensive while ARPU is low.
- Segment 3 contract conversion incentives may compress margins and create discount dependency.

This tradeoff framing was critical for an executive-level presentation.

### **If I had more time, I would:**
- Tune CatBoost and boosting models more systematically (grid search / Bayesian tuning)
- Add threshold optimization (profit-based or cost-based thresholding instead of default 0.5)
- Create a simple business simulation showing expected ROI from targeting each segment
- Expand explainability using SHAP plots to strengthen stakeholder confidence

---

## Supporting Materials Included

This folder includes:
- `Case Competition - Notes and Models.ipynb` (my model experiments + notes)
- `Executive Summary.pdf` (final project narrative)
- `Recommendation Notes.pdf` (segment recommendations + tradeoffs)
- `k- mean segmentation.xlsx` (segmentation output + supporting analysis)
