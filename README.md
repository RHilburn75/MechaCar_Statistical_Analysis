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

![image](https://user-images.githubusercontent.com/94253815/158034823-7a8adea6-2ec4-4899-b4be-1071ec66850d.png)













## Study Design: MechaCar vs Competition
