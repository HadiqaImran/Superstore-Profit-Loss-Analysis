# Superstore Profit Analysis

## Overview
This project investigates what is actually driving profit loss in a retail superstore. The central hypothesis was that heavy discounting is the primary villain — and the data confirmed it, with some additional surprises.

## Business Question
**What is driving profit loss, and what should the business do about it?**

## Dataset
Kaggle Superstore Sales Dataset — 9,994 orders across 4 regions, 3 categories, and 17 sub-categories in the United States.

## Tools & Technologies
- Python (Pandas, Matplotlib, Scikit-learn)
- Power BI
- Jupyter Notebook

## Project Structure
- **EDA** — Profit breakdown by category, sub-category, region, and state
- **Discount Analysis** — Bucketed discount ranges and their impact on profit and loss rate
- **Linear Regression** — Predicting profit and identifying which variables matter most
- **Power BI Dashboard** — 4-page interactive dashboard with KPIs, visuals, and a recommendations table

## Key Findings
- 18.72% of all orders are loss-making — systemic, not random
- Discounts above 20% consistently produce negative profit; the 40–60% bucket has nearly 100% loss rate
- Discount has a coefficient of -191 in the regression model — the single strongest predictor of profit loss
- Tables and Bookcases are structurally loss-making even without heavy discounting
- Copiers are the strongest profit driver across all sub-categories
- Central region has the lowest profit margin at 7.9% vs West at 14.9%

## Model Note
Linear regression R² of 0.19 — the model confirms discount as the dominant variable, but profit is influenced by many factors beyond what's captured here. The low R² is expected given the complexity of retail pricing dynamics.

## Recommendations
| Finding | Recommendation | Evidence |
|---|---|---|
| 19% of orders lose money | Audit discount approval process | 1 in 5 orders is loss-making |
| Discounts above 20% destroy profit | Cap discounts company-wide at 20% | 40–60% bucket near 100% loss rate |
| Central region margin only 7.9% | Investigate regional pricing and logistics | West margin is 14.9% on similar products |
| Tables & Bookcases structurally loss-making | Review supplier costs or discontinue | Negative profit even without heavy discounting |
| Copiers are highest profit driver | Prioritize copier sales and marketing | Strongest positive variable in regression |
