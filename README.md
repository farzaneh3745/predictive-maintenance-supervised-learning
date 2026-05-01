# Predictive Maintenance Supervised Learning Assignment

This repository contains seven self-contained Jupyter notebooks, one for each research question.

## Dataset
The notebooks expect the raw dataset file at:

`../data/predictive_maintenance_cleaned_New.csv`

Each notebook also tries `/mnt/data/predictive_maintenance_cleaned_New.csv` as a fallback.

## Target
`failure_within_24h`

## Task Type
Binary classification for industrial predictive maintenance.

## Outputs
Each notebook saves:
- One CSV table in `../results/tables/`
- One PDF figure in `../results/figures/`

## Research Questions
1. Baseline performance
2. Model comparison
3. Effect of preprocessing
4. Feature importance and interpretability
5. Sensitivity to evaluation metrics
6. Robustness and generalization
7. Practical usefulness and final recommendation

## Notes
- Possible leakage columns are excluded from prediction: `rul_hours`, `failure_type`, and `estimated_repair_cost`.
- Figures and tables are generated from actual dataset results after running the notebooks.
- If `xgboost` is unavailable, notebooks fall back to scikit-learn Gradient Boosting.
