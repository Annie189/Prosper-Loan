# Prosper Loan Data Exploration

## Dataset

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others
The dataset can be found here:
https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1554486256021000

Atrribute definition can be found here: https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0

As there are a lot of attributes (81 attributes) in the dataset, the student would like to focus on the trends and relationships between following attributes:

- Borrower APR
- Borrower Rate
- Lender Yield & Estimated Yield
- Estimated Loss
- Prosper Score & Rating
- Income Range & Employment Status
- Term & Loan status
- Occupation & State
- The student would like do deep into univariate, binvariate and multivariate exploration to answer following questions:

- Which values is the domniant in each attributes regarding count of loans?
- Which are the trends between attributes? Which insights can we find out from that?
- Which factors are important to Borrower APR? (The student especially focus on this attribute sine it is a key role in loan transactions)

## Summary of Findings
1. Regarding Prosper Score & Rating:

- ProsperScore has negative relationship with BorrowerAPR, LenderYield, Estimated Effective Yield and Loss. This show that lower score means higher risks and hence higher interest rates, higher the lender earns and higher risk of loss.
- Prosper Rating tends to have positive relationship with Credit Score. Higher credit score will lead to better Prosper rating and vice versa.
- Most loans with lower BorrowerAPR & LenderYield have higher ProsperScore and visa-versa.

2. Regarding Loan Orginal AmounT and Borrower APR:

Loan Original Amount has positive relationship with Prosper Score but both of them have negative relationship with Borrower APR. Higher prosper score will get lower borrower APR. Also, most of the loans with higher amounts (>$20,000) are taken by people with higher prosper score (10 and above)

3. Regarding employment status, prosper score and borrower APR:

- Most borrowing transactions are made by employed and full-time individual
- Full-Time and part-time tend to have higher ProsperScore and lower BorrowerAPR
- Not-Employed & Self-Employed tend to have lower ProsperScore and higher BorrowerAPR
- Retired people have higher ProsperScore and lower BorrowerAPR
- Employed people are diverse regarding the ProsperScore and BorrowerAPR

4. Regarding loan status:

Most of the loans are current, some are completed. Just a few of them are charged off or defaulted. Gathering two variables as a heatmap, we can see that current loans which are taken by employed people are the dominant percentage of the total loans. Another big cluster of taking loans are those working full time had completed loan (17397 transactions).

Past Due loans generally have higher interest rates in all employment statuses. Part time, Retired or Not employ tend to have higher rate than those with full-time job or being employed.

5. Regarding Listing Category, debt consolidation are the one have most loans. Most current loans are in debt consolidation. Most completed loans are also in deb consolidation.

6. Regarding Income Range, borrower APR was likely to be higher in low income or not employed group.


## Key Insights for Presentation

For the presentation, I focus on the relationship between Borrower APR and other important factors including: Lender Yield, Prosper Score, Income Range, Employment Status, Loan Status.... I start by introducing the
borrower APR distribution, followed by plots and heatmaps with other relationships so that we can have an overview of how other factors are important to borrower APR. From that, we are confident to conclude significant insights.
