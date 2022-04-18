# Module 15: Statistics and R
Use R to help MechaCar that is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team. to create data visualization tools. Tableau can be used to transform your data into an engaging story for any audience.

## Overview of the analysis:
- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Linear Regression to Predict MPG.

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

- The variable with the best relation is "vehicle_length". We can confirm with the scatter plot and in the correlation matrix.


Image# 1
![Image# 1](https://user-images.githubusercontent.com/95668609/163743617-ff2271b4-b253-4c99-bda0-9da86533d21f.png)


Image# 2
![Image# 2](https://user-images.githubusercontent.com/95668609/163743624-744eb495-2045-4d08-a414-15ee5a7fb3ec.png)


Is the slope of the linear model considered to be zero? Why or why not?

- We have many values close to 0 and others not as close to 0 as the previous ones. So we can it depends on the coefficients you are looking at some are very close to 0.


Image# 3
![Image# 3](https://user-images.githubusercontent.com/95668609/163743654-8fe69494-fefb-4a31-8d4c-41cfebb3eb3b.png)


Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

- According to the p-value and the r squared, the model does explain most of variations.
* The r-squared is 0.7149, closer to 1 than 0.


Image# 4
![Image# 4](https://user-images.githubusercontent.com/95668609/163743671-6a6d4125-bb4a-4187-9079-98ce4d307f6d.png)


# Summary:  
The linear regression provides sufficient visualization on the relation between vehicle_length to the mpg values in the dataset. 
As greater the vehicle the mpg will be higher.

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 

- Total summary indicates that the condition is not greater than 100 pounds per square inch.


Image# 5
![Image# 5](https://user-images.githubusercontent.com/95668609/163743680-c4eb619a-2924-4a20-b6d7-78fa6e64baea.png)


- When values are grouped by batch we realize that lot 3 is the only one that does not comply with the condition that is not greater than 100 pounds per square inch.


Image# 6
![Image# 6](https://user-images.githubusercontent.com/95668609/163743688-449cb4a4-50cb-434d-8961-ba5695ce0c0c.png)


Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

- Looking at the Total Summary, the overall variance is under 100 psi, while the lot summary shows the variance for lot 3 is obove the tolerance at 170.28 psi.

## T-Test on Suspension Coils

- If our significance level was the common 0.05 percent, our p-value general is above our significance level.


Image# 7
![Image# 7](https://user-images.githubusercontent.com/95668609/163743696-022b99c9-9912-4ce5-a1ec-81cc28c7e3d4.png)


- Looking at the data for each batch we can notice that one and two are statistically similar, however, the third is not.


Image# 8
![Image# 8](https://user-images.githubusercontent.com/95668609/163743706-5bfc8137-33e8-467c-8a48-74b53aa0ed02.png)


## Design a Study Comparing the MechaCar to the Competition

- The location must be consideres as the social stratum to which we aim and will affect the metrics to be used.
- We assum the consumer is middle-class in a populated urban area.
- After an online search consumers are usually based on the following points.

Metrics

- Car security.
- Fuel efficiency.
- Low maintenance cost.
- Price.
- Environmentally friendly.
- Calm driving.

Hypothesis

- Alternative Hypothesis: Metrics described influence the consumer when making his choice.
- Null Hypothesis: Metrics described do not affect the choice of our products or those of the competition.

Test the hypothesis

- The significance level should be taken as 5% to mitigate type 1 error.
- Take multiple samples to have points of comparison.
- Test on one sample test of the mean of the samples if they correspond to the population.
     

