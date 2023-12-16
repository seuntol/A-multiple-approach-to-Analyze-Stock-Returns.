# A-multiple-approach-to-Analyze-Stock-Returns.

## Aim of Project
This aim of this presentation is to guide Mr. John Hughes undertsand:
The effect of dividend on stock_return_scaled using a linear regression model
The effect of return, market_overview, dividend, earnings_ranking, debt_to_equity and marketcap on stock_return_scaled using a multivariate regression model.
Methodology
The research will use the r-programming language to acertain the basic statistics and develop an histogram of stock_return_scaled. We would go further to conduct a T-test to ascertain if the mean of stock_return_scaled is equal to 300.
A linear regression model will developed using dividend as my independent variable and stock_return_scaled as our dependent.
A multiple regerssion analysis will also be carried out using all input variables as our independent variable and stock_return_scaled as our dependent.
From the evidence of our analysis, we will state our conclusions and give insight to Mr John Hughes data set.   

## Understanding the dataset
In order to carry out any data analysis it is important to understand some basic key statistics of your dataset; they range from Measure of Average to the Measure of Dispersion to other statistics such as the Minimum value, the maximum value. We also need to identify variables that are not numerical, hence cannot have means and some other statistics
Measure of Average
Mean is the sum of all the data divided by the number of observation
Median is the middle value when the data is arranged in a sized order 
Mode is the most common data value
Measure of Dispersion : This measures the spread of the data set .
Variance: It is a statistical measure of how far the numbers are spread in a dataset from their average 
Standard Deviation: The standard deviation measures the dispersion of the values in a dataset from their mean. It is the square root of the Variance 
Other Statistics
Minimum: This is the minimum value in the dataset
Maximum: This is the maximum value in the dataset.
Range: The difference between the Maximum and Minimum

## T test
We will be running a one sample two tailed two test to determine if the mean of our dependent variable is equal to 300. We have a known mean value but the population standard deviation is not known hence the use of a one sample mean. It will be a two tailed test because we are trying to ascertain if there is equality with the known mean implying the value could be either greater or lower.

Assumptions of the test:
• Data is independent. 
• Data is collected randomly.
• The data is approximately normally distributed 

## Simple Linear Regression
The Simple linear regression is used to ascertain if there is a significant relationship between the dependent variable and a single independent variables. It will adopt the t test to determine if the generated coefficient is statistically significant and an F statistics to evaluate the overall model.

Conditions for the Least Squares Line The following conditions must be satisfied for fitting a least squares line

Linearity There should be a linear relationship between the variables that are used to fit the model. 

Nearly normal residuals The residuals should be nearly normal. 

Constant variability The variability of the points with respect to the least squares line should be nearly constant. 

Independent observations The observations used in the linear regression should be independent. 

### Steps for Linear Regression
Hypothesis Statement t test for coefficient and F test for overall model

		Ho: β=0, co-efficient β of the predictor is zero and not statistically significant
		Ha: β ≠0, co-efficient β of the predictor is not equal to zero and is statistically 			significant 						
2. Significance Level
We will be adopting a significance level of 0.05
3. Perform a Simple Linear Agression in R
Load my dataset
Build my model; inputting my codes in R and getting the outputs
4. Evaluate the result by comparing the p-value with the significant level
Compare the p-value with the significant level to ascertain which is greater hence deciding if the independent variable is relevanting to the model (t-test) and the overall model (F-statistics) to decide if there is siginificant evidence to fail to reject or reject the null hypothesis
5. State my conclusion 
Clearly state what the result of my test infers. In this test, with a p value of 0.801 which is greater than the significant level of 0.05, I can say there is no sufficient evidence to reject the null hypothesis; thus I fail to reject the null hypothesis that states that the co-efficient β of the predictor is zero and not statistically significant.

## Multivariate Regression
The Multiple linear regression is used to ascertain if there is a relationship between the dependent variable and multiple independent variables. It will adopt the t test to determine if the generated coefficients are statistically significant and an F statistics to evaluate the overall model.

The multi variate models have similar "LINE" assumptions like the simple linear regression stated in the slides above. However, with multiple linear regression we have to think of the distribution of errors at a fixed set of values for all the predictors.

### Steps for MultiVariate Regression
Steps in Analyzing a Multiple Regression Model 
Collect the sample data i.e., y, x1, x2, . . . , xk for each experimental or observational unit in the sample 
Hypothesize the form of the model. This involves choosing which independent variables to include in the model 
Use the method of least squares to estimate the unknown parameters β0, β1, ... ,βk
Statistically evaluate the utility of the model 
Check that assumptions of the model are satisfied and make model modifications if necessary 
Finally, if the model is deemed adequate, use the fitted model to estimate the mean value of y or to predict a particular value of y for given values of the independent variables, and to make other inferences

## Conclusion
The model developed to use a simple linear regression to ascertain the effect of dividend on stock_return_scaled showed with the t test that the dividend variable was not statistical significant and the F statistic p-value showed that the overall model was not significant. We fail to reject both the t test null hypothesis and the F statistics null hypothesis for this model because their p-value was greater than the signifcance level of 0.05.
The Multiple Linear Regression showed that marketoverviewneutral, marketoverview positive, debt to equity and marketcap are statistically significant and are a good predictor of stock return scaled. However return, dividend and earnings ranking are not statistically significant to be good predictors of stock return scaled. We considered dropping them to improve the precision of the model. We fail to reject the t test null hypothesis for the independent variables that were not statistically significant because of their p value was greater than the significance level and rejected the t test null hypothesis for both the statistical significant variable and the F statistics null hypothesis for this model because their p-value was less than the signifcance level of 0.05.

Using the Adjusted R approach, the result shows The effect of dividend on is not significant using the Simple Linear Regression Model
The effect of marketoverviewneutral, marketoverview positive, debt to equity and marketcap is significant while return, dividend and earnings ranking is not significant using the Multivariate Linear Regression Model.
The overall evaluation of the simple regression model is not significant, the overall evaluation of the mulivariate regression model is significant.
We therefore advise Our Client to adopt the Multivariate regression model over the linear regression model. 
Mr John can also improve the precison of the model by considering dropping return, dividend and earnings ranking.
Also worthy of note is that marketoverview and dividend are categorical variable and may be theoretical right but not pratically useable. Further investigations is therefore needed.

the multiple linear regression model has a better predictor having a higher value of 63.2% compared to the single linear regression with a very low Adjusted R.









