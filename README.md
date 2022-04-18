# Module 15: Statistics and R
Use R to help MechaCar that is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team. to create data visualization tools. Tableau can be used to transform your data into an engaging story for any audience.

## Overview of the analysis:
- Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

## Results: 

## Linear Regression to Predict MPG.

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

- The variable with the best relation is "vehicle_length". We can confirm with the scatter plot and in the correlation matrix.

Image# 1

![Image# 1](https://user-images.githubusercontent.com/95668609/163744186-996ad18e-d4ce-4cf3-9860-69c4016bed58.png)

Image# 2
![Image# 2](https://user-images.githubusercontent.com/95668609/163744192-69cf8e26-b492-4c75-b47a-2f552d305bbf.png)


Is the slope of the linear model considered to be zero? Why or why not?

- We have many values close to 0 and others not as close to 0 as the previous ones. So we can it depends on the coefficients you are looking at some are very close to 0.

Image# 3
![Image# 3](https://user-images.githubusercontent.com/95668609/163744199-6229bf0e-9e42-4ece-ae20-d99989c8ced9.png)


Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

- According to the p-value and the r squared, the model does explain most of variations.
* The r-squared is 0.7149, closer to 1 than 0.

Image# 4
![Image# 4](https://user-images.githubusercontent.com/95668609/163744210-add93417-1c46-45d4-8490-b5898da3e7e6.png)


# Summary:  
The linear regression provides sufficient visualization on the relation between vehicle_length to the mpg values in the dataset. 
As greater the vehicle the mpg will be higher.

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 

- Total summary indicates that the condition is not greater than 100 pounds per square inch.

Image# 5
![Image# 5](https://user-images.githubusercontent.com/95668609/163744216-6e23ab64-0ee4-474f-8e57-ea65cc66a567.png)


- When values are grouped by batch we realize that lot 3 is the only one that does not comply with the condition that is not greater than 100 pounds per square inch.

Image# 6
![Image# 6](https://user-images.githubusercontent.com/95668609/163744221-9430b3e6-36e2-495f-be84-0b48a56b8579.png)


Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

- Looking at the Total Summary, the overall variance is under 100 psi, while the lot summary shows the variance for lot 3 is obove the tolerance at 170.28 psi.

## T-Test on Suspension Coils

- If our significance level was the common 0.05 percent, our p-value general is above our significance level.

Image# 7
![Image# 7](https://user-images.githubusercontent.com/95668609/163744224-41c359d9-91a1-4ace-a3a8-b564328efe0e.png)


- Looking at the data for each batch we can notice that one and two are statistically similar, however, the third is not.

Image# 8
![Image# 8](https://user-images.githubusercontent.com/95668609/163744229-38406b38-97ec-4aa0-b9bc-1b01d87716e4.png)


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
     
Neccesary data

- We need the most data available posible to analyze and project trends.
- The best is to have at least 10 years of information with specific location that is expressed to take it into consideration.
- We need to understatnd big event that will affect our data. Take into consideration Covid-19 phase that hit the automovil industry, as well as other factors suchs as war, oil price increases, etc.
