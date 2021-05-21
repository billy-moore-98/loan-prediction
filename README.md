# loan-prediction

Credit modelling is important in determining risk when investing in potential loans. If a borrower does not pay their loan back on time, the investor will lose money.

In this project I have taken Lending Club loan data from 2007 to 2011. The data contains information on various loans, most of which were paid back on time and some which were defaulted. The data can be found [here](https://www.kaggle.com/wordsforthewise/lending-club).

The aim is to build a machine learning model that will accurately predict whether a potential borrower will pay their loan back on time. In this context the true positive and false positive rates are important.
If we invest in a false positive, we will lose money.

The dataset also had a high positive class imbalance. To deal with this class penalties, threshold moving and synthetic minority oversampling (SMOTE) were explored.

It was found that the best model for the aim was a logistic regression model with balanced class weights. The logistic regression model with SMOTE didn't perform as well.
The model has a good balance of true positive and false positive rates, such that an investor can be relatively confident that if they invest in a loan the model predicts to be paid back on time,
they will not lose money.

If the notebooks do not render please use [Jupyter nbviewer](https://nbviewer.jupyter.org/).
