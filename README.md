# Bank Marketing Classification — Assignment 17.1

This project compares K-Nearest Neighbors (KNN), Logistic Regression, Decision Tree, and Support Vector Machine (SVM) classifiers for predicting whether customers subscribe to a term deposit during telephone marketing campaigns.

## Business objective
Use historical campaign data to help prioritize outreach. The target is `y` (`yes`/ `no`).

## Files
- `Bank_Marketing_Classification_Assignment.ipynb` — end-to-end analysis, data preparation, classifier comparison, evaluation, interpretation prompts, and recommendations.
- `requirements.txt` — Python dependencies.
- `.gitignore` — standard Python/Jupyter ignores.

## Run
1. Install dependencies: `pip install -r requirements.txt`
2. Open the notebook: `jupyter notebook Bank_Marketing_Classification_Assignment.ipynb`
3. Run all cells. If automatic download is blocked, download the official Bank Marketing archive from https://archive.ics.uci.edu/dataset/222/bank+marketing and place `bank-additional-full.csv` in the notebook directory.

## Methodology
- Stratified train/test split with fixed random seed.
- One-hot encoding and imputation for categorical features; imputation and standardization for numeric features.
- Preprocessing is performed inside scikit-learn pipelines.
- `duration` is excluded because it is only known after the call and is not a valid pre-call feature.
- Comparison includes precision, recall, F1, ROC-AUC, confusion matrices, and stratified cross-validation.

## Before submitting
Run every notebook cell and replace the generic interpretation prompts with conclusions supported by actual outputs. The notebook has not been pre-run in GitHub, so do not report performance numbers until you have run it. Submit this public repository URL: https://github.com/subhransupanigrahi/bank-marketing-classification

## Data source
UCI Machine Learning Repository, [Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing).
