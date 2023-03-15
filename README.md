# WineSatisfaction-Logistic Regression Analysis

Performed a simple multiple linear regression model on a dataset containing properties of wine and customer quality rating and
satisfaction. Using the WineSatisfaction.csv dataset, I ascertained if pH, alcohol, and price influence
customer perception of quality. 

Results:

![wine data](https://user-images.githubusercontent.com/114897374/225187347-d5568fbf-b0ff-4006-a42e-55760921ae90.png)


The alcohol content  and retail price of the wine influence the customer perception of quality with p-values of 0.0019 and 0.0001 respectively.
The pH however does not statistically influence the customer perception of wine quality because it has a p-value of 0.2463.
The p-value for the model: 0.0001 shows that the model overall can be trusted and the properties influence the customer perception of the quality of wine.

b.	Explaining the R-Square 

A value of 0.3870 for R-squared indicates that approximately 38.70% of the variation in the dependent variable is explained by the independent variable(s) in the model. 
This means that Alcohol, pH and Price influences only 38.70% of the customer perception of the quality of wine. The remaining 61.30% may be influenced by the other properties of wine, customer quality rating and satisfaction that are not included in the analysis.

c.	Estimating Quality Rating of a Wine Bottle

Based on the results, a bottle of wine with the following properties:
i.	pH =3.5
ii.	price = $8.50
iii.	alcohol = 9.5
will have a Quality rating of 5.22 based on the calculation below:
=     Intercept + (alcohol slope * alcohol content) + (pH slope * pH property) + (price slope * retail    price)
=     5.0058 +( - 0.0408*9.5) + ( - 0.0753*3.5) + (0.1021*8.5)
=     5.2225


# WineSatisfaction-Logistic Confusion Matrix

![wine confusionmatrix](https://user-images.githubusercontent.com/114897374/225187931-708843f1-8796-4ccf-93d0-f4c76d8f24b6.png)


True Negative: 
●	These are the instances where our model correctly predicted that the Loan customer defaulted on the loan.
●	Here, our model correctly predicts that 6961 out  of the 9000 loan customers in the Testing data defaulted on their loans
False Negative: 
●	This shows the number of instances our model predicted that the Loan customer defaulted on their loan  when the actual data showed that the customer repaid the loan in time.
●	Out of the sample of 9000, the model falsely predicted that 1882 defaulted on their loans.
True Positive:
●	These are the number of instances that our model correctly predicted that the loan customer repaid the loan. 
●	Here, the model correctly predicted that 110 of the 9000 customers repaid their loans.
False Positive: 
●	These are the number of instances that our model predicted the loan customer repaid on the loan when they actually defaulted. 
●	Our model predicted that 48 customers out of the 9000 repaid  their loan when the actual data showed that they defaulted on their loans.

Accuracy
(TP+TN/(TP+TN+FP+FN)
=    (110+6961)/(110+6961+48+1882)
=    0.7856

Precision
TP/(TP+FP)
=    110/(110+48)
=    0.6962

Recall
TP/(TP+FN)
=    110/(110+1882)
=    0.0552



