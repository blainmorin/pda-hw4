# pda-hw4

1. Wells in Bangladesh used for drinking are often contaminated by natural arsenic which can cause diseases as exposure accumulates in someone’s body. If someone’s well is contaminated, a neighbor’s well may be safe and so if they agree, one can switch to sharing their well. After a research team measured arsenic levels in all the wells in a certain area, residents were urged to switch wells if theirs was labelled unsafe (more than 0.5 hundred micrograms per liter, i.e. 50 micrograms). A few years later the researchers returned to see who had switched wells. The data are in the file wells.txt, found in the data sets folder. They include 5 variables for 3020 wells

switch is a binary indicator for whether the household switched wells

arsenic is the level of arsenic in the well in hundreds of micrograms per liter

dist is the distance to the nearest safe well in meters

assoc is whether household members are active in community organizations

educ is the number of years of education of the head of household.

First construct a training data set of the first 2520 wells and a test data set of the last 500.

a. Construct a good logistic regression model predicting the decision to switch wells as a function of the 4 predictors (arsenic, distance, association and education) on the training data. Consider potential transformations of continuous variables and possible interactions.

b. Compute and graph the predicted probabilities stratifying by the predictors. You could do this using graphs such as in the papers we discussed in class or by using contour plots which would allow you to graph two continuous predictors on the same plot. You can array different lines and plots to try to put this all on one sheet or you can spread across different plots. See what works best.

c. Compute the confusion matrix on the test data using p = 0.5 as a cutoff and discuss what this tells you about the predictive model you have constructed (e.g. sensitivity, specificity, error rate, etc.)

d. Construct an ROC plot and compute the area under the ROC curve.

e. What does this curve tell you about choice of threshold that balances sensitivity with specificity (i.e., how would you balance risk of switching and not switching?)

f. Repeat this analysis using linear discriminant analysis, quadratic discriminant analysis and K nearest neighbor with K = 1 and K = 5. For discriminant analysis, note that the predict function returns 3 elements: class is a binary indicator as to whether the posterior probability is greater than 0.5, posterior gives the posterior predictive probability and x contains the linear discriminant for the LDA function (missing for QDA). Note that for KNN, you will only get classifications, not probabilities.

 

2. (Extra credit for biostat PhD students). Do exercise 2.9 in Hastie and Tibshirani.