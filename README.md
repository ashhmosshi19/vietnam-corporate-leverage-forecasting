# Forecasting Corporate Leverage in Vietnam

A time-aware machine-learning study of leverage forecasting and a rule-based financial-distress proxy for Vietnamese listed companies.

## Approach

- feature engineering from lagged financial ratios;
- time-based train/test separation;
- regression and classification baselines;
- comparison of Ridge, Random Forest, and Gradient Boosting models;
- evaluation with both predictive metrics and business interpretation.

The main analysis is in `notebooks/leverage_pipeline.ipynb`.

## Result snapshot

The recorded notebook run reports approximately 0.779 classification accuracy for its Random Forest distress-proxy experiment. The metric is dataset- and split-specific; it is not a claim about future market performance.

## Data and limitations

The source Excel files are not included because their redistribution rights are unclear. To reproduce the notebook, provide an authorized copy and update the input path. The target is a rule-based proxy, not a clinical or regulatory definition of financial distress. Small samples, reporting delays, survivorship effects, and sector differences can materially affect the result.

```bash
python -m pip install jupyter numpy pandas scikit-learn matplotlib openpyxl
```
