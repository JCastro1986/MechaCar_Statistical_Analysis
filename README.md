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
![Image# 1](https://user-images.githubusercontent.com/95668609/165003759-43a43090-fc58-47fc-abd9-423864f45405.png)


Image# 2
![Image# 2](https://user-images.githubusercontent.com/95668609/165003767-b0b3cbe9-bfbd-49e6-bd60-dabfaf16a214.png)


Is the slope of the linear model considered to be zero? Why or why not?

- We have many values close to 0 and others not as close to 0 as the previous ones. So we can it depends on the coefficients you are looking at some are very close to 0.

Image# 3
![Image# 3](https://user-images.githubusercontent.com/95668609/165003773-ec177eaf-2929-4f06-a1d2-2a5c5c1e7271.png)


Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

- According to the p-value and the r squared, the model does explain most of variations.
* The r-squared is 0.7149, closer to 1 than 0.

Image# 4
![Image# 4](https://user-images.githubusercontent.com/95668609/165003779-17ad6c6c-d916-4d5b-879c-9a7c769c7780.png)


# Summary:  
The linear regression provides sufficient visualization on the relation between vehicle_length to the mpg values in the dataset. 
As greater the vehicle the mpg will be higher.

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 

- Total summary indicates that the condition is not greater than 100 pounds per square inch.

Image# 5
![Image# 5](https://user-images.githubusercontent.com/95668609/165003784-9765c59f-e4c3-4b7d-afff-19fd8138759a.png)


- When values are grouped by batch we realize that lot 3 is the only one that does not comply with the condition that is not greater than 100 pounds per square inch.

Image# 6
![Image# 6](https://user-images.githubusercontent.com/95668609/165003788-d7143bf8-f722-4166-aa68-016eadf66415.png)


Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

- Looking at the Total Summary, the overall variance is under 100 psi, while the lot summary shows the variance for lot 3 is obove the tolerance at 170.28 psi.

## T-Test on Suspension Coils

- If our significance level was the common 0.05 percent, our p-value general is above our significance level.

Image# 7
![Image# 7 1](https://user-images.githubusercontent.com/95668609/165003800-558fcf8e-1339-4d51-b476-ee26ba3a09f0.png)


- Looking at the data for each batch we can notice that one and two are statistically similar, however, the third is not.

Image# 8
![Image# 8 1](https://user-images.githubusercontent.com/95668609/165003809-42429cf6-76cb-47c3-93b4-38baf33566ec.png)


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
