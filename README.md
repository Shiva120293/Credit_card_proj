# Credit_card_proj


**Abstract**


In recent years, the credit card issuers in Taiwan faced the cash and credit card debt
crisis and the delinquency is expected to peak in the third quarter of 2006
(Chou,2006).
In order to increase market share, card-issuing banks in Taiwan over-issued cash
and credit cards to unqualified applicants. At the same time, most cardholders,
irrespective of their repayment ability, overused credit card for consumption and
accumulated heavy credit and cash–card debts.
The crisis caused the blow to consumer finance confidence and it is a big challenge
for both banks and cardholders.


**Problem Statement**


This project is aimed at predicting the case of customers default payments in
Taiwan. From the perspective of risk management, the result of predictive
accuracy of the estimated probability of default will be more valuable than the
binary result of classification - credible or not credible clients.
We can use the K-S chart to evaluate which customers will default on their credit
card payments.


**Dataset Summary**


**Attribute Information:**


This research employed a binary variable, default payment (Yes = 1, No = 0), as
the response variable. This study reviewed the literature and used the following 23
variables as explanatory variables:


X1: Amount of the given credit (NT dollar): it includes both the individual
consumer credit and his/her family (supplementary) credit.

X2: Gender (1 = male; 2 = female).

X3: Education (1 = graduate school; 2 = university; 3 = high school; 4 = others).

X4: Marital status (1 = married; 2 = single; 3 = others).

X5: Age (year).

X6 - X11: History of past payment. We tracked the past monthly payment records
(from April to September, 2005) as follows:
X6 = the repayment status in September, 2005;

X7 = the repayment status in August, 2005; . . .;

X11 = the repayment status in April, 2005. The measurement scale for the
repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment
delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay
for nine months and above.

X12-X17: Amount of bill statement (NT dollar).

X12 = amount of bill statement in September, 2005;

X13 = amount of bill statement in August, 2005; . . .;

X17 = amount of bill statement in April, 2005.

X18-X23: Amount of previous payment (NT dollar).

X18 = amount paid in September, 2005;

X19 = amount paid in August, 2005; . . .;

X23 = amount paid in April, 2005.

**Steps involved:**

1. Importing important libraries to be used.
 
2. Mounting the drive and loading the dataset.
 
3. Exploratory data Ana
 
4. Data extraction and manipulation.
 
5. Splitting the data using Train
 
6. Fitting the dataset over various models like logistic regression, forest, KNN, Stochastic Gradient Descent.


**Logistic Regression**


In Logistic Regression, we wish to model a dependent variable(Y) in terms of one
or more independent variables(X). It is a method for classification. This algorithm
is used for the dependent variable that is Categorical. Y is modeled using a
function that gives output between 0 and 1 for all values of X. In Logistic
Regression, the Sigmoid (aka Logistic).

**Conclusion**

Our best prediction accuracy was around 88-89%, our lowest measured
prediction accuracy was about 13%. This is not a particularly large
spread, especially considering the disparity in the time it takes for some
models to train with the Grid Search to find the best hyper-parameters.
we streamlined the training and prediction process very well, but despite
the feature engineering, and hyper parameter tuning we didn't see a
particularly significant change in predictive power of our models.
If we were to make recommendation to a crediting agency about the
granting of credit, with respect to the debtors likelihood to default, it
would be:


Consider the applicants marital status. Married people seem to
default more often.

Consider the age of the applicant. Younger people are at higher
risk of defaulting.

Establish a lower limit balance for applicants that would be
considered risky.

Once granted credit, pay special attention to the ratio of payments
to the amount owed on their balance. There will be some threshold
were it's very unlikely that they will be able to pay you back.

Limit the number of months a debtor may be late on their
payments to 3, like most credit agencies. At this point it's more
likely that the person will default than pay you back. At this point
you're only giving more money away.
.
