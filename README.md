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
 
 The slope of the linear model cannot be considered zero. The p-value of the linear regression analysis is 5.35e-11, which is smaller than the assumed acceptance level of 0.05%. Because of this, there is no significant evidence to reject the null hypothesis, meaning our slope of the linear model is not zero.







## Summary Statistics on Suspension Coils


## T-Tests on Suspension Coils


## Study Design: MechaCar vs Competition
