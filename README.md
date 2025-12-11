# predictive-patent-dashboard
A tool for innovators and lawyer to input information about their patent to predict the likelihood of it to be approved. Trained on data from US Patent and Trademark office.

This project is an interactive Streamlit dashboard developed as part of a project examining how USPTO Office Actions influence the likelihood that a patent application receives an allowance.

The dashboard combines:
- Exploratory Data Analysis (EDA) across USPTO Technology Centers
- A trained XGBoost predictive model estimating allowance probability
- Scenario testing tools for evaluating how specific rejection patterns, citation counts, and application characteristics impact outcomes

**Model Details:**
- Model Type: XGBoost Classifier
- Version: xgboost == 3.1.2
- Training Data: Historical USPTO Office Action dataset from US Patent and Trademark office
- Target Variable: Probability of allowance
- Feature Inputs:
  1) Rejection codes
  2) Citation counts
  3) Severity metrics
  4) Application characteristics
  5) Examiner / Tech Center information

Note: This tool provides statistical insights, not legal advice.
Predictions are based on historical data and should not be interpreted as definitive outcomes.
