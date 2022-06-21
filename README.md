# (Prosper Loans Exploration)
## by Akingbeni David


## Dataset

> The prosper loan dataset is a table of 130K+ entries and 81 columns that are called features. These features dynamically provide information on each loan entry and specific information such as the borrower's APR, loan status e.t.c. This dataset was among the optional datasets that Udacity provided for data vizulization project,from which I chose I chose this beacuse of my flair for the world of finance, retail and business.
> The dataset contained a number of missing values that were replaced by negative values to  show that they were missing values rather than drop them because of some other features that such particular row might possess.
> A notable wrangling process would be the combination of the Credit Grade and ProsperRating column which were actually credir rating grades but from different sources.
> The dataset conatains so many features but I had to eventually choose only a subset of 30-40 columns and made use of only around 10 columns in the entire analysis.


## Summary of Findings

> The summary of the finding is split into two main features which were the ProsperRating and the LoanStatus of a loan.
> The effect of income on the assigned rating and income class who borrowed most adn the effect of other features on the dataset.
> At first we discovered that there was almost the same count of numbers of high risk and low risk loans, i.e. by count both type of loans received almos the same attention, we went on and realize that while that is true, higher risk loans are usually less than 6,000.
> The most active borrowers were within the 2K to 10K
> Also there is a shift in the income and loan borowed  to entities in recent years and Prosper Loans now take more safely rated loans than before.


## Key Insights for Presentation

>- The effect of the Loan Amount on Prosper rating. At first when we explore the count of the prosperrating we discover that low risk and high risk loans have almos the same number of loans given out. On further exploration with the boxplot distribution of the LoanAmount and Prosperrating, we discover that the Most High Risk loans are lower than high risk loans as the median loan amount reduces as the risk increases. The violin plot does show the distribution better.
>- The effect of the DebttoIncome Ratio and ProsperRating depending on the loanStatus. The Debt ToIncome ratio on initial comparism when we use a facetgrid to compare the distribution between the different loan status does not show any difference to explore, however when we use a pointplot of the debt to income ratio by the different prosperrating and use the hue as the loan status, we identify a converging debt to income ratio as the risk increases which meant that as the risk increases the debt to income ratio flexibility for any loan decreases.
>- The effect of Income, Loan Amount and LoanStatus is a dynamic interaction with different contributing factors. At first the interaction between the income and loan amount does give us little information about loan activities and amount associated with different income range. As we do explore the further we discover that a range of other information affects the loan status. One of the two important refrence information is the interaction between Income, Rating and Loan Status(After subsetting the year range to not include 2013 and above) - that tells that higher income earners in high risk category(D-HR) complete their loans than defaulters. This trend is also true for AA rated loans but is silent for loans of income earners with ratings between (A - C).
> The second reference equation is the interaction between the loan amount, rating and loan status which there is a high range of loan amount borrowed for low risk loans and the difference between defaulters and those who completed their loans converge as the risk increases. This means that as the loan gets highly risky, the rating of the loan and income of the earner determines whether a loan will be defaulted or not, and the loan amount plays little role among the defaulters (They are not borrowed much anyways). As the risk reduces however i.e(HR back to AA), the amount borrowed plays a key role in whether the loan will be defaulted or not.