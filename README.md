# MechaCar_Statistical_Analysis

# Deliverable 1
## Linear Regression to Predict MPG

Deliverable Requirements:
The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using your knowledge of R, you’ll design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file.

Requirements:

* _The MechaCar_mpg.csv file is imported and read into a dataframe_
* _An RScript is written for a linear regression model to be performed on all six variables_
* _An RScript is written to create the statistical summary of the linear regression model with the intended p-values_
* _There is a summary that addresses all three questions_

#### Results on Deliverable:
###### Resulting Model:

mpg = (6.267)vehicle_length + (0.0012)vehicle_weight + (0.0688)spoiler_angle + (3.546)ground_clearance + (-3.411)AWD + (-104.0)
 
#### Written Summary
_1. We got in vehicle length and vehicle ground are statistically likely to provide non-random amounts of variance to the model. that means that vehicle length and vehicle
ground clearance have an impact talking about miles per gallon on the MechaCar prototype. in the other hand, vehicle weight, spoiler angle, and AWD have p-values that indicate
random amount of variance in the dataset._

_2. In this case slope of this linear model is not Zero becase the p-value = 5.35e-11, compared with assumed significance level 0.05% indicate there is sufficient evidence to
reject our null hypothesis._

_3. For this linear model has an r-squared: 0.7149, that means approximately 71% of all mpg predictions that will be determined by this model. in this way, his multiple
regression model predict mpg of MechaCar prototypes in god way and effectively._

   ####  Model Image Results
   ![](https://github.com/JulioAQuintana/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)
  
  # Deliverable 2
  ## Summary Statistics on Suspension Coils
The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to
determine if the manufacturing process is consistent across production lots. Using your knowledge of R, you’ll create a summary statistics table to show:

* _The suspension coil’s PSI continuous variable across all manufacturing lots_
* _The following PSI metrics for each lot: mean, median, variance, and standard deviation._

Requirements:
* _The Suspension_Coil.csv file is imported and read into a dataframe_
* _RScript is written to create a total summary dataframe that has the mean, median, variance, and standard deviation of the PSI for all manufacturing lots_
* _An RScript is written to create a lot summary dataframe that has the mean, median, variance, and standard deviation for each manufacturing lot_
* _There is a summary that addresses the design specification requirement for all the manufacturing lots and each lot individually_

#### Results on Deliverable 2:
Suspension Coil dataset provided for the MechaCar contains the results of testing the weight capacities of multiple suspension coils and from multiple production lots to
determine consistency.

  ### Fist calculation of Manufacturing lot:
   ![](https://github.com/JulioAQuintana/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

  ### and then analysis by each one of 3 manufacturing lots:
   ![](https://github.com/JulioAQuintana/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

* _The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current_
* _manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?_

during the analysis of entire population of the production lot, we got variance of the coils at 62.29 PSI, within 100 PSI variance requirement. in the other hand and in
consistent trend, Lot 1 and Lot 2 are in good way within the 100 PSI variance requirement, with variances of 0.98 and 7.47 respectively, the Lot 3 that showa larger variance in
performance and consistency, with a variance of 170.29, It is Lot 3 that is disproportionately causing variance in the complete lot level.

  # Deliverable 3
  ## T-Tests on Suspension Coils
Using your knowledge of R, perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds
per square inch.

Requirements:
* _An RScript is written for t-test that compares all manufacturing lots against mean PSI of the population_
* _An RScript is written for three t-tests that compare each manufacturing lot against mean PSI of the population_
* _There is a summary of the t-test results across all manufacturing lots and for each lot_

#### Results on Deliverable 3:
The next step is to conduct a t-test on the suspension coil data to determine whether there is a statistical difference between the mean of this provided sample dataset and a
hypothesized, potential population dataset. Using the presumed population mean of 1500, we find the following:

There is a summary of the t-test results across all manufacturing lots:

   ![](https://github.com/JulioAQuintana/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)
   
based on the information we got we can see the true mean of the sample is 1498.78. With a p-value of 0.06 that is higher than the common
significance level of 0.05, we assume that is not enough evidence to support rejecting the null hypothesis, also we can see in the analysis that the mean of all three of these
manufacturing lots is statistically similar to the population mean of 1500.

so based at each individual lots:

_1. Lot 1 has true sample mean of 1500, again as we saw in the summary statistics above. With a p-value of 1, clearly we cannot reject the null
hypothesis.
_2. Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean
of 1500 are statistically similar. implícitaimp
_3. Lot 3 has a different result scenario, here the sample mean is 1496.14 and the p-Value is 0.04 lower than the common significance level of 0.05. All
indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different.

  ![](https://github.com/JulioAQuintana/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)
  
After this analysis, the recomendation is to perform a revision of lot 3 due that we probably have some fails in the production system.

  # Deliverable 4
  ## Study Design: MechaCar vs Competition
Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

Requirements:
* _A metric to be tested is mentioned_
* _A null hypothesis or an alternative hypothesis is described_
* _A statistical test is described to test the hypothesis_
* _The data for the statistical test is described_

#### Results on Deliverable 4:
Analysis would imply the data collection for comparable models by MechaCar that will be compared other
manufacturers in the last years, we have to design in base a typo of models comparables, what car
models could be compared under the same conditions, and what models will be included in the loop under
the similar prices.

Important Metrics

Data collection of competitors comparable models during last years in order to cover the important metrics:

* _Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable_
* _Recall history (claims): Independent Variable_
* _Current Price (Selling): Dependent Variable_
* _Drive Package : Independent Variable_
* _Resale Value: Independent Variable_
* _Safety Feature Rating: Independent Variable_
* _Average Annual Cost of ownership (Maintenance): Independent Variable_
* _Gas effieciency: Independent Variable_

#### Decription of A null hypothesis or an alternative hypothesis

based on key factors defined of MechaCars genere we shape the following Hypothesis

Null Hypothesis: The prices of MechaCar are correctly rated based on performance of key factors forits 
genre.
Alternative Hypothesis: MechaCar have NOT rated priced correctly based on performance of key factors
for its genre.

#### Statistical Tests description to Hypothesis

we have to perform multiple linear regression in this case will be used to determine the factors that have the highest impacts, correlation and forecast with the list selling price that is a dependent variable, probably all of them has a lot of impact in the price base on the statistic. 
