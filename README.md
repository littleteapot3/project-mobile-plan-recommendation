# Megaline Plan Recommender 📱

This project builds a machine learning model to recommend one of two modern mobile plans—Smart or Ultra—for Megaline subscribers based on their monthly usage behavior.

## Project Goal

Megaline, a telecom provider, wants to migrate users from legacy plans to modern offerings. The goal is to develop a model that can accurately predict whether a subscriber should be offered the **Smart** or **Ultra** plan, using historical behavioral data.

🎯 **Target accuracy**: ≥ 0.75  
✅ **Best model**: Random Forest (Test Accuracy: 0.83)

## Dataset

Each row contains one user's monthly usage:
- `calls` — number of calls made
- `minutes` — total duration of calls
- `messages` — number of text messages sent
- `mb_used` — internet traffic in MB
- `is_ultra` — actual plan used (Ultra = 1, Smart = 0)

## Key Steps

- Performed exploratory data analysis (EDA) with visualizations
- Compared three models: **Logistic Regression**, **Decision Tree**, and **Random Forest**
- Evaluated model performance using validation accuracy
- Tested the final model on an unseen test set
- Built a baseline "if-then" rules-based model for comparison

## Results

| Model                | Validation Accuracy |
|---------------------|---------------------|
| Logistic Regression | 0.74                |
| Decision Tree       | 0.72                |
| Random Forest       | **0.84 ✅**         |

- Random Forest outperformed simpler models and captured complex relationships in the data.
- A baseline threshold-based model performed no better than chance (50%).

## Next Steps

- Add cross-validation for greater robustness
- Explore additional features like account age, payment behavior, or customer location

---

## Notebook

➡️ Check out the full notebook: [`mobile_plan_recs.ipynb`](./mobile_plan_recs.ipynb)

---
