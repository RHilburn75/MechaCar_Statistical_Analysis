# MechaCar_Statistical_Analysis

MechaCar, the newest prototype from AutosRUs, is suffering from productiond problems, which is causing setbacks in the progression of the manufacturing teams progress. Upper management has asked Jeremy and his data analytics team to review the production data for any insights that will help the manufacturing team get back on track.

There are 4 parts of the project that will be analized and data shown this report:

 1. Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
 2. Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
 3. Run t-tests to determine if the manufacturing lots are statistically different from the mean population
 4. Run t-tests to determine if the manufacturing lots are statistically different from the mean population
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG

  We first performed a multiple linear regression analysis to determine which variables the MPG.  Using Summary(), we were able to determine the p-value and the r-squared value for the linear regression model.
  
![image](https://user-images.githubusercontent.com/94253815/158033587-6eec934f-a42c-4e64-b276-3b4dd51a3899.png)
  
![image](https://user-images.githubusercontent.com/94253815/158033735-28b59175-2130-4f95-9663-05e76c1cae53.png)

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
 
  Vehicle_length and ground_clearence are least likley to provide the amount of variance to the mpg value because these two variables have and impact on mpg values.

2. Is the slope of the linear model considered to be zero? Why or why not?
 
   The slope of the linear model cannot be considered zero. The p-value of the linear regression analysis is 5.35e-11, which is smaller than the assumed acceptance level of    0.05%. Because of this, there is no significant evidence to reject the null hypothesis, meaning our slope of the linear model is not zero.

3.  Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

   The r-squred value is 0.7149 (71.49%), meaning the variability of the dependant variable mpg is explained by the linear expression module. The results show the linear module predicts mpg of MechaCar prototypes positively.
   
## Summary Statistics on Suspension Coils

There were 2 summaries created in this section to summarize the statistics on PSI of the suspension coils from the manufacturing lots.  The charts are below.

This chart is a summary for the entire manufacturing site.

![image](https://user-images.githubusercontent.com/94253815/158034319-fb3e1da6-654d-421c-ad63-b4a49c14a6aa.png)


This chart shows the summary for each manufacturing lot

![image](https://user-images.githubusercontent.com/94253815/158034369-171b7857-ad5c-466e-be58-37a86970619b.png)

1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

 - Looking at the total_summary, the variance is 62.29, which indicates the current manifacturer doesn't meet the design specification that the variance of the suspension coils be within 100 pounds per square inch.

Not all lots mee the requirement
 - Lot 1 - Variance of 0.98
 - Lot 2 - Variance of 7.46
 - Lots 1 and 2 do meet the design specification requirement.
 - Lot 3 - variance of 170.29, which is over the requirement.  
 Because of the results, Lot 3 is over the requirement, and as a result, does not meet the requirement.

## T-Tests on Suspension Coils

We had to perform t- tests to determine if the manufacturing lots are different from the population mean.

1. This T-test is created to determine the PSI across all manufacuturing lots is different from the population mean of 1500pounds per square inch.

![image](https://user-images.githubusercontent.com/94253815/158034873-86690d8f-a9c9-493d-8fde-6daa1b47ed1c.png)
 - P-Value = 0.06028 which is greater than our assumed level of 0.05.  Because of this, we do not have enough evidence to reject the null hypothesis.
 - Accept the null hypothesis and and reject the alternative hypothesis
 The PSI across all manufacturing lots are statistically similar to the population mean of 1,500 pounds per square inch.

The following three t- test are used to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 PSI.

Manufacturing Lot 1

![image](https://user-images.githubusercontent.com/94253815/158034948-c222a8c7-0b73-415b-9209-5f695afe3e72.png)

 - The p-value from this test is 1,  which is greater than our assumed acceptance level of 0.05, but it also indicates the observed mean is exactly the same as the population mean.
 - We can conclude that the PSI  for manufacturing lot 1 equals the population mean of 1,500 PSI.
 
 Manufacturing lot 2
 
![image](https://user-images.githubusercontent.com/94253815/158034989-d97858e8-538e-4426-90de-0cdf62e6f2c6.png)

 - The p- value from this t- test is 0.06072 - greater than our assumed level of 0.05.  We do not have evidence to reject the null hypothesis.
 - The PSI for manufacturing lot 2 is similar to the population mean of 1,500 PSI.

Manufacturing lot 3

![image](https://user-images.githubusercontent.com/94253815/158035014-d94af203-7910-4707-810c-1a8953d1ced7.png)

 - The p-value from the t -test for lot 3 is 0.04168 - smaller than our assumed level of 0.05
 - We do have evidence to reject the null hypothesis and accept the alternative hypothesis.
 - Lot 3 is not equal to 1,500 PSI


## Study Design: MechaCar vs Competition

For the final section we put together a study of some key metrics and some statistical studies on how the MechaCar would compare to the competition.  The below will state the metrics to measure, the hypothesis, the test we would use, and the data compiled and used to support our hypothesis.

1. What metric or metrics are we going to test?

 - Cost
 - Fuel Effeciency
 
 I feel these are the top 2 metrics consumers want to know when buying an automobile, especially during these times. Car prices have increased since the pandemic started, due to the high demand and lack of inventory With the increase in the cost of gas, fuel effeciency is quickly becoming the main topic of car discussion.
 
 2. What is the null hypothesis or alternative hypothesis?
 
 Cost:
 
 Null Hypothesis:  The means of cost of all vehicles in this class are equal.
 
 Alternative Hypothesis: At least one of the vehicles  in this class has a different mean of cost than other vehicles.
 
Fuel Efficiency:

Null Hypothesis:  The means of fuel efficiency of all vehicles in this class are equal.
 
Alternative Hypothesis: At least one of the vehicles in this class has a different mean of fuel efficiency than other vehicles.

3. What statistical test would you use to test the hypothesis? And why?

We'll use the ANOVA test for this study, because ANOVA test is ued to compare the means of continuious numerical variable across multiple groups.

Cost:

One-Way ANOVA test. This test will be used to test the mean cost of MechaCar with multiple competition vehicles' mean cost in the same class

Fuel Efficiency:

Two Way ANOVA test. This test will be used to test the mean of fuel efficiency of MechaCar with multiple competition vehicles' mean fuel efficiency in the same class

4. What data is needed to run the statistical test?

 - Sample size of 50-100 MechaCars, along with 50-100 samples of the competitors vehicles.  This would complete a sufficient analysis.
 - For cost, we would sample the same vehicles to find the mean fule efficiency.


