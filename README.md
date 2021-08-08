# MechaCar_Statistical_Analysis

## Tools ans Resources

**Source:** *MechaCar_mpg.csv* and *`Suspension_Coil.csv`*
**Tools and Software:**  *`tidyverse`, `dplyr`, `MechaCarChallenge.RScript`, `RStudio`* and *`R`.*

## Objective

You are approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on you to review the production data for insights that may help the manufacturing team.

## Linear Regression to Predict MPG

*Insert Slide0 Here*

From the above output we can see that:

1. The "vehicle length", and "vehicle ground clearance" are statistically likely to provide non-random amounts of variance to the model. The vehicle shape and ground clearance will
have an impact on gas mileage for the prototype.   

2. The p-Value, is much smaller than the assumed level of 0.05% which rejects our null hypothesis and concludes that the linear slope is "not zero".


3. 71% of all mpg predictions is determined in this model, represented by the r-squared value and the model does 
predict mpg of MechaCar prototypes effectively. 

When we remove variables like "All Wheel Drive", "spoiler angle", and "vehicle weight", the predictability doesn't dramatically decrease noted by the r-squared value of decline from 0.7149 to 0.674. 

*Insert Slide1 Here*

## Summary Statistics on Suspension Coil

The Suspension Coil dataset provides the MechaCar results for testing the weight capacities of multiple suspension coils from multiple production lots to determine consistency.

In the first image shows the total summmary of all manufacturing lots


*Insert Slide 2 Here*


This next image, breaks down the our analysis by viewing the data by Lots.


*Insert Slide 3 Here*



If we look at the entire population of the production lot, the variance of the coils is 62.29 PSI, which is within the 100 PSI variance requirement. Lot 1 and Lot 2 are well within the 100 PSI variance requirements but Lot 3 has a much larger variance in performance and consistency, with a variance of 170.29. Lot 3 has the largest diviation which impacts the overall proformance data for all lots.

## T-Tests on Suspension Coils


### t-test results across all lots

*Insert Slide 4 Here*



Looking at the overall manufacturing there is NOT enough evidence to support rejecting the null hypothesis, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.


The Image below is the t-test result of each manufactured lot.


*Insert Slide 5 Here*



The summary shows something went wrong in Lot 3's production and the process needs to be reviewed for production failures.


## Study Design: MechaCar vs Competition

#### Metrics
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

Safety Feature Rating, Current Price (Selling),Drive Package, Engine (Electric, Hybrid, Gasoline / Conventional), Maintenance, MPG (Gasoline Efficiency)


#### Hypothesis: Null and Alternative
After determining which factors are key for the MechaCar's genre:

 * Null Hypothesis (Ho): MechaCar is priced correctly based on its performance.
 * Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance.
 
#### Statistical Tests
The **multiple linear regression** would be used to determine the factors that have the highest correlation/predictability with the list selling price!


