# Bank Loan Risk Classifier

A bank wants to automate their loan approval process.  They have provided a semi-anonymized dataset containing 606 successful and 76 not successful loans along with their information and transactions. These loans are for existing clients. This could be used to pre-approve existing customers and market to them accordingly.

This analysis looks into a dataset from a Czech bank. The goal here is to produce a model that can predict whether client is high-risk for a bank loan.

Original with the data dictionary: [link](https://sorry.vse.cz/~berka/challenge/pkdd1999/berka.htm)

In the data table `loan.csv`, the data from the different tables was preprocessed where the transaction data was aggregated by monthly amount.

## Prerequisite

The notebook, `bank_loan.ipynb`, is written in Python 3. The libraries that are used in this notebook are listed under the `requirements.txt` file. One can simply issue to following command to insure the proper libraries are installed:

```bash
pip3 install -r requirements.txt
```

## Description of analysis

The analysis consists of a brief explanatory analysis where distributions of predictors were examined. It also consists of how the bank loan risk was modeled using a random forest classifier where a F1-score of 85% on predicting high-risk clients. SHAP analysis was performed to further understand how the main predictors that impact the model output and to obtain insights for business recommendations. Adjusting the class weights was necessary to resolve the imbalance issue of the original data set. Summary of results were put together and can be found in the `slides.pdf` in this repo.
