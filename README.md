# Statistical-Inference-for-Big-Data (in R)

The problem
Like all firms, life insurance companies continually seek new ways to deliver products to the market. Those
involved in product development wish to know “who buys insurance and how much do they buy?” Analysts
can readily get information on characteristics of current customers through company databases. Potential
customers, those that do not have insurance with the company, are often the main focus for expanding
market share.

We examine the Survey of Consumer Finances (SCF), a nationally representative sample that contains ex-
tensive information on assets, liabilities, income, and demographic characteristics of those sampled (potential

U.S. customers). We study a random sample of households with positive incomes that were interviewed in
the 2018 survey.
For term life insurance, the quantity of insurance is measured by the policy (FACE), the amount that the
company will pay in the event of the death of the named insured. For those customers who still do not have
any life insurance this value is set to zero.
Characteristics that might turn out to be important include annual INCOME, the number of years of
EDUCATION of the survey respondent and the number of household members, NUMHH, the GENDER,
the marital status MARSTAT, the charitable contributions, CHARITY.

1

Variable Description

GENDER Gender of the survey respondent

AGE Age of the survey respondent

MARSTAT Marital status (=1 married,=2 living with partner, =0 otherwise)

EDUCATION Number of years of education of the survey respondent

ETHNICITY Ethnicity

SMARSTAT Marital status of the respondent’s spouse

SGENDER Gender of the respondent’s spouse

SAGE Age of the respondent’s spouse

SEDUCATION Education of the respondent’s spouse

NUMHH Number of household members

INCOME Annual income of the family

TOTINCOME Total income

CHARITY Charitable contributions

FACE Amount the company will pay in case of the death of the named insured

FACECVLIFEPOLICIES Face amount of life insurance policy with a cash value

CASHCVLIFEPOLICIES Cash value of life insurance policy with a cash value

BORROWCVLIFEPOL Net amount at risk on life insurance policy with a cash value

Question 1 (6pt)
1. Import the data set in a data frame (the final object should be a tibble).
2. Produce a new data frame (to be used later for the data analysis) by selecting only the dependent
variable and the other variables that might be of interest, as reported in the description of the problem.
3. Do all the operations you think are useful to get a clean the data set.
Question 2 (6pt)
1. Implement an R function that reads a data frame, counts the number of missing values in each variable
and produce as an output a vector with the number of missing values. Better, produce a named vector
with the name of the variables in the data set and the corresponding number of missing values.
2. Apply your function to the dataset imported at point 1 of the previous question and, briefly, comment
the results.
Question 3 (6pt)
1. Construct a new variable to identify the customers that already have a life insurance and those that
still do not have one.
2. Compare the two gropus with respect to the income. Is there any difference between the two groups?
(hint: consider both EDA and inferential tools).
3. What are your comments?


Question 4 (6pt)
1. What is the relationship between the “quantity of insurance” and the income? Note that the analysis
makes sense only if conditioned on those customers who already have a life insurance. (hint: consider
both EDA and inferential tools).
2. Repeteat the previous analysis by conditiong on the gender of the costumer.
Question 5 (6pt)
Study the relationship that links the amount that the company will pay in the event of the death of the named
insured with some of its characteritic: the annual income, the number of years of education, the number of
household members, the gender and the marital status. What are your comments for the insurance company,
given the estimated model? Note that the analysis makes sense only if conditioned to the those who already
have a life insurance.
