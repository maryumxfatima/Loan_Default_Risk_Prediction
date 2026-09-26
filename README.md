# Loan Default Risk Prediction

Capstone project by Team 1 for the Circle x DataCamp program.

This project predicts whether a loan applicant will default, using their application plus their full financial history across seven connected data tables (Home Credit Default Risk dataset from Kaggle).

## About the Project

Home Credit lends to people with little or no credit history. We cleaned and joined the seven tables, created new features from each applicant's credit and payment history, and trained models to predict default. Since only about 8% of applicants default, we used ROC-AUC instead of accuracy to measure performance.

We started with a logistic regression baseline using only the main application table (ROC-AUC 0.749). Our final gradient boosting model, using all seven tables, reached a ROC-AUC of 0.782 on unseen test data.

The most important factors were external credit scores, how the loan is structured, past repayment behaviour, credit card utilisation and debt at other banks.

## How to Run
1. Download the dataset from [Kaggle: Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk) and place all CSV files in a folder named `data`, in the same directory as the notebook.
2. Open the notebook in Jupyter Notebook/Lab.
3. Change this line near the top of the notebook to match where the project folder is saved on your own computer:
```python
   os.chdir(r'C:\Users\Lenovo\Desktop\loan_default_project')   # change address only to the data on your comp
```
4. Run all cells from top to bottom (Kernel → Restart & Run All).

Libraries used: pandas, numpy, scikit-learn, scipy, matplotlib, seaborn

## Team
Aiman and Hareeba (data cleaning and joining), Zainab (feature engineering), Maryam (modelling and evaluation)
