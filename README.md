# suicidal-children
Classification Project

My classification project was about children’s mental health in the Western Pacific. Each year, 25% of global suicides 
occur in the Western Pacific and youth suicide rates are even higher there. When I did some research on that topic,
I found that islands like Samoa and Guam in the Western Pacific had some of the highest suicide rates of youth.
I decided to collect my data from the Global School-based health survey conducted by the World Health Organization.

 I made my target as whether or not a child has considered attempting suicide in the past 12 months and my features
 as country facts and the rest of the survey data excluding some similar questions related to suicide. What I found 
 is that about 13% of children surveyed in the Western Pacific has considered attempting suicide in the past 12 months.
 When using logistic regression, I mitigated this class imbalance by introducing class weights. When I used an
 XGBoost model, I decreased the threshold for my positive class. 

Interesting things I found from my data was related to the article I read about suicide rates in the Western Pacific. 
I found that although Kiribati was the highest risk island, with more than ⅓ of surveyed children considering suicide
in the past year, Samoa was also part of the top 3 high risk countries. 

How did my models do to predict whether or not a child will be suicidal? My logistic regression and XGboost model
returned similar results, but XGBoost had a slightly higher F1 score of .44. In retrospect, I should have chosen 
an F2 score, where I weigh recall more since it is better to catch all children who might be suicidal.
But, nonetheless, I was able to find out which survey questions had the most weight using feature importance.
I found out that the questions that had the most weight also appeared to be significant questions in my logistic 
regression model. 

The questions that had the most weight were if the child felt lonely, if the child had insomnia from worrying, 
if the child has been bullied, and if the child has tried cigarettes at a young age. The more lonely a child felt, 
the more sleep a child loses over excessive worrying, the fact that a child was bullied, and the fact that a child
has tried cigarettes at a younger age was correlated with the child being suicidal. 
