# MechaCar_Statistical_Analysis
Module 15: Statistics and R

## Overview of Project
A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. F

## Results
### Deliverable 1: Linear Regression to Predict MPG

The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using  R, We have to design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file.


- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
 The vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. 

- Is the slope of the linear model considered to be zero? Why or why not?
Due to p-Value: 5.35e-11, is smaller than the significance level of 0.05%. There is enough evidence to reject our null hypothesis, so that the slope of this linear model is not zero.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Yes, this linear model has an r-squared value of 0.7149, this represents 71% of accurary at all mpg predictions will be determined by this model. 
 

![image](https://user-images.githubusercontent.com/90117562/152737858-e5cf9104-4b11-4d06-9121-4101035a7298.png)


![image](https://user-images.githubusercontent.com/90117562/152739336-b6df48d7-5d12-4c85-888e-423fdbdfc169.png)


### Deliverable 2: Summary Statistics on Suspension Coils

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:
-  The suspension coil’s PSI continuous variable across all manufacturing lots
-  The following PSI metrics for each lot: mean, median, variance, and standard deviation.

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
The Lot 1 variance is 0.979 while Lot 2 shows a variance of 7.469 which means that those Lot do not exceed 100 pounds per square. However, the unique Lot that do not meet the design specification is Lot 3 with a Variance of 170.28

![image](https://user-images.githubusercontent.com/90117562/152744210-dcf941b9-d9c0-4859-b72f-d7c3707df0bc.png)

![image](https://user-images.githubusercontent.com/90117562/152744232-3209fab6-0cc3-4231-80be-97b5379a2f56.png)


### Deliverable 3: T-Test on Suspension Coils

- Using R, I performed t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

The p-Value of 0.06 is higher than the significance level of 0.05 so that there is NOT enough evidence to support rejecting the null hypothesis.

![image](https://user-images.githubusercontent.com/90117562/152746852-b4e70af4-5749-4009-a3b5-6f72db80961b.png)

Lot 1 sample with a p-Value of 1, so we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean of 1500

![image](https://user-images.githubusercontent.com/90117562/152746895-b22dcca6-c9da-4e56-a19f-f28e28381019.png)

Lot 2 has shows a p-Value of 0.61 which says that the null hypothesis cannot be rejected.

![image](https://user-images.githubusercontent.com/90117562/152746926-e8130a09-e227-4f72-8644-a612b4c2d1f4.png)

Lot 3 shows a sample mean of 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. These results demands to reject the null hypothesis, because the means are not statistically similar.

![image](https://user-images.githubusercontent.com/90117562/152746966-580d7ef5-2f9a-49eb-9b2f-1effc9dc1ea8.png)
