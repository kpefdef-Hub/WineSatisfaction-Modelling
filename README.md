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


# WineSatisfaction-T Test (1-tail test)

![Screenshot (57)](https://user-images.githubusercontent.com/114897374/225190343-7e1381ab-b440-440d-a584-72b1ba26e235.png)

The p-value of the T test is less than the confidence level of 0.05 at 2.44403452210091E-22 which means the analysis is significant. 
The mean value for the Customer perception of the quality of White wine at 5.88 is higher than the mean for Red wine which is 5.64. The negative t-stat also supports us that the Customer perception of White wine is greater than for Red wine. 
Therefore, we reject the null hypothesis that the Customer perception of the quality of red wine is the same as white wine.






