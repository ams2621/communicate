# ProsperLoan Data Exploration

## Dataset

This data set (https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1547699802003000)
contains 113,937 loans with 81 variables on each loan, including loan amount, 
borrower rate (or interest rate), current loan status, borrower income, and many others.
This [data dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit?usp=sharing) explains the 
variables in the data set.
The project objective is not expected to explore all of the variables in the dataset! But focus on only exploration on about 10-15 of them.
#### I have taken 16 variables to do my analysis and a subset of around 76000 rows.


## Summary of Findings:
I'm most interested in figuring out what features are best for predicting the borrower's Annual Percentage Rate (APR) for the loan and how employment status and debtToIncome ratio associates with various metrics in the dataset. 
1. LoanStatus of all Borrowers are with current and completed state.
2. The distribution of monthly income of applicants is a right skewed because there will be few applicants with high salary. 
3. LoanStatus with current and completed have own homes when they applied for loans
4. we can see there is around 55 % borrower who own a home and rest don't have their own house.
5. I found that the most popular services offered by Prosper are Debt Consolidation, Home Improvement, and Business having a count of more than 10000, other categories have a count of less than 10000
6. Interestingly we can observe thatThe borrower APR decreases with the better rating. Borrowers with the best Prosper ratings have the lowest APR. It means that the Prosper rating has a strong effect on borrower APR. 
7. From the above plot we can depict that for employed, self employed and full time borrower rarte is around 0.2. Further we can observe that borrowers who are employed and full - time have a monthly income in the range of 10000 to 20000 above that are outliers.

## Key Insights for Presentation:
I start by looking at the distrbuiton of each and every numeric and categorical variables and did all the necessary univariate, bivariate and
mulitvariate analysis on the selected varaibles.
1. From the visualization we can easily depict that Borrower APR is multimodal having a sharp peak between 0.35 and 0.38, further we can observe that there is peak (small) at 0.1 as well as at 0.3.
2. ProsperRating is an ordinal categorical variable defined by Prosper using historical data, with the following values from higher to lower ('AA', 'A', 'B', 'C', 'D', 'E', 'HR'), ratings have almost normal distribution in data set centered at 'C' which is having the maximum count the highest 'AA' and the lowest 'HR' ratings have the lowest counts
3. From the following plots we can depict how Borrower APR depends on Term, Prosper Rating(Alpha) and Debt to Income Ratio. Interestingly we can observe thatThe borrower APR decreases with the better rating. Borrowers with the best Prosper ratings have the lowest APR. It means that the Prosper rating has a strong effect on borrower APR.
4. From the visualization we can observe that for HR there is only 36 month loans with a mean borrower apr as 0.35, further it increases from B to AA category, and is maximum for the AA category around 0.10 
#### At the end I would conclude that Borrower APR highly negatively correlated with variables, further we can say that loan status of a borrower is also dependent on its employment status, stated monthly income as well as he has his own house or not futher even on his monthly loan payment. Eventually if he has higher monthly income loan can be easliy paid by making high loan payment

## Limitation:
The Exploratory Data Analysis is a good way to know the data using vivid and interesting visualizations. However, to make final statement about the  relationships among variables we need to conduct statistical test and  build predictive models.


```python

```
