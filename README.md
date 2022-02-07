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

Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

In your README, create a subheading then briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.


### Deliverable 4: Design a Study Comparing the MechaCar to the Competition




Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.
In your description, address the following questions:
What metric or metrics are you going to test?
What is the null hypothesis or alternative hypothesis?
What statistical test would you use to test the hypothesis? And why?
What data is needed to run the statistical test?
