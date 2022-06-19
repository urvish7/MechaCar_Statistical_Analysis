# MechaCar_Statistical_Analysis
## Overview of the Project:

A few weeks after starting a new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team

In this challenge, you’ll help Jeremy and the data analytics team do the following:

 - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
 - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
 - Run t-tests to determine if the manufacturing lots are statistically different from the mean population
 - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

Please Find the code file under the below link:

[MechaCarChallenge.R](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/MechaCarChallenge.R)

## Deliverable 1: Linear Regression to Predict MPG
  
The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using the knowledge of R, you’ll design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file.


### Linear Regression to Predict MPG
![](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/ScreenShots/mechacar_mpg.png)

### An RScript is written for a linear regression model to be performed on all six variables 
![](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/ScreenShots/Six_Variables.png)

The three takeaways :
 - Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
      - The non-random variable's variance for the most time is O, the coefficient of the intercept, ground clearance and vehicle length can be provided non-random amount of the variance to the MPG values.
 - Is the slope of the linear model considered to be zero? Why or why not?
      - The P-value: 5.35e-11, is much smaller than the assumed significance level of 0.05%. According to the analysis it is been indicated that the results lean towards the reject the null hypothesis, at the linear model would be zero. 
 - Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
      -  Regression model: The multiple R-squared of .71 indicates the relation however multiple R-square is incrementing as more variable passed through the regression. With the increment in R-valueor getting the high, the linear model predict mpg effectively.  


## Summary Statistics on Suspension Coils


The Total Summary Data:

![](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/ScreenShots/total_summary.png)

From the total_summary data, the overall variance of all the lots that meets the manufacturing data design specification have the variance 62. The mean, Median,and Std_Dev are at 1498.78 , 1500 , and 7.892627 respectively. 


The Lot Summary Data:

![](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/ScreenShots/lot_summary.png)

The Lot3 variance is way superior than the Lot2 and Lot1. while when it comes to the Means and Median the value of Lot3 is inferior than the Lot1 and Lot2. 

## T-Tests on Suspension Coils

Performing a t-test on the suspension coil data. This process is to determine the statistical difference between the mean of the sample dataset and hypothesized potential population dataset by using a presumed population mean of 1500. 

![](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/ScreenShots/t_test.png)

The data shows the p-value is 0.06 which is more than common signifiance level of 0.05, so it wont be suffient to support rejecting the null hypothesis. 


The Three Lots individual results with the t-test:

![](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/ScreenShots/t-test_lot1-lot2.png)
![](https://github.com/urvish7/MechaCar_Statistical_Analysis/blob/main/ScreenShots/t-test-lot3.png)

 - Lot1 : The significance level is 0.05, failed to reject the null hypothesis throwing the p-value equals 1. Also as the p-value increases, the confidence interval decreases.
 - Lot2 : The significance level is 0.05, failed to reject null hypothesis throwing the p-value equals 0.61.
 - Lot3 : The significance level is 0.05, failed to reject null hypothesis throwing the p-value equals 0.04. 

## Study Design: MechaCar vs Competition

### What metric or metrics are you going to test?

  MechaCar needs to adapt the statistical approach to manage the               depreciation on the vehicle. 
  The metrics shows the depreciation rate over the life of the vehicle.

### What is the null hypothesis or alternative hypothesis?

  When it comes to Null hypothesis, there is no statistical difference         between the rate of depreciation for the MechaCar and the Copetition.

### What statistical test would you use to test the hypothesis? And why?

  The Statics shows that the analysts at MechaCar need to use the linear       regression, as this would show the depreciation over time. 

### What data is needed to run the statistical test?

  Age Mileage condition make model.











