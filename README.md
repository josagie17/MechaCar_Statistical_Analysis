Jeremy gets approached by top management about a unique project a few weeks after starting his new job. The MechaCar, AutosRUs' newest prototype, is experiencing production issues that are impeding the manufacturing team's development. Upper management at AutosRUs has asked Jeremy and the data analytics team to evaluate production data for insights that might benefit the manufacturing team. In this challenge, I will assist Jeremy and the data analytics team in completing the following tasks:

Conduct multiple linear regression analysis to determine which characteristics in the dataset predict MechaCar prototype mpg.

Obtain summary information on the pounds per square inch (PSI) of suspension coils from manufacturing lots.

Use t-tests to see if the manufacturing lots differ significantly from the average population.

Create a statistical research to compare the performance of MechaCar cars to other manufacturers' vehicles. I will produce a concise explanation of the findings for each statistical analysis.

Deliverable 1 – Linear Regression to Predict MPG

Ground clearance and vehicle length, as well as vehicle weight to a lesser extent, are statistically unlikely to supply random amounts of variation to the linear model, implying that all three factors have a considerable influence on MechaCar mpg. The probability coefficient (Pr(>|t|) value for the ground clearance, vehicle length, and vehicle weight variables are all reduced. The other factors, spoiler angle and AWD, appear to add a random amount of variation to the linear model, as seen by their greater probability coefficients.

The linear model's slope is not taken to be zero.This is because the p-Value is computed to be 5.35e-11, which indicates the likelihood that a statistical measure will be larger than or equal to 0, or, to put it another way, the possibility that we will find identical results if we test our data again. The expected (normal) p-value of 0.05 is much less than the 5.35e-11 p-value. This indicates that the chances of being mistaken about the randomness of these variables are quite low.

Approximately 71.4 percent of the time, the linear model accurately predicts miles per gallon (mpg). This is based on the determined r-squared value, which in this case was 0.7149, which indicates how well the regression model predicts real-world data and ranges from 0 to 1, with 0 representing no prediction and 1 representing total predictability. The correlation strength is strong in this situation, as seen by the r-squared value of 0.7149.

<img width="929" alt="Deliverable1 1" src="https://user-images.githubusercontent.com/92246505/158685917-b8ec4b14-f4bf-4b63-87e6-13d46463e5f2.png">


Deliverable 2 - Summary Statistics on Suspension Coils:

The suspension coils' deviation could not exceed 100 pounds per square inch, according to the design criteria for the MechaCar suspension coils. The variance overall variance for all three lots was 62.29356, which is considerably below the 100-psi criterion, according to the total summary dataframe that was produced. On a per-lot level, however, the variance does differ by lot number, as seen in the lot summary dataframe. Lot 1 has a variation of 0.9795918 and Lot 2 has a variance of 7.4693878, both of which are within the variance tolerance of 100 psi.

However, Lot 3 has a significantly greater variance of 170.2861224, which exceeds the design requirements' variance tolerance. This implies that Lot 3 will have to be removed from manufacturing, while Lot 1 and Lot 2 will be able to be used.

<img width="531" alt="Deliverable 2 1" src="https://user-images.githubusercontent.com/92246505/158686093-39802a96-4f21-4e68-b1f3-bce3b14cbce0.png">

<img width="576" alt="Deliverable 2 2" src="https://user-images.githubusercontent.com/92246505/158686132-fbdfd6d8-dd3e-4dc2-8a74-15541e7184e2.png">

Deliverable 3 - T-Tests on Suspension Coils:

The p-value for the combine lot t-test is 0.06028, which is higher than the conventional significance limit of 0.05, indicating that there is no meaningful linear connection and that the PSI impact is due to random chance and error. Finally, because there is insufficient evidence to justify its rejection, the null hypothesis must be accepted (the null hypothesis is failed to be rejected).

Lot No. 1: Lot 1 has a p-value of 1, indicating a very significant connection between the Lot 1 PSI and the population mean of 1500 PSI. The fact that the Mean PSI for Lot 1 was 1500 further supports this, proving that there is no statistical difference between the Lot 1 sample and the population mean.

Lot No. 2: Lot 2 has a p-value of 0.6072, indicating a substantial connection between the Lot 2 PSI and the population mean of 1500 PSI once again. Lot 2's Mean PSI was 1500.20, which is nearly identical to the population mean of 1500. We must also fail to reject the null hypothesis, as we did in Lot 1.

Lot No. 3: Lot 3 differs from the other two lots in terms of representation. Because it differs so much from Lot 1 and Lot 2, it has a significant influence on the total p-value for the combined lots, as indicated by the fact that it has far more variation than the other two lots. We must reject the null hypothesis based on the p-value of 0.04168, as the data reveals that the sample PSI of Lot 3 and the population mean have a very weak association.

<img width="540" alt="Deliverable 3 1" src="https://user-images.githubusercontent.com/92246505/158686251-3c2c2b8f-49da-429d-8a89-d6e6e5a14f01.png">

<img width="933" alt="Deliverable3 2 1" src="https://user-images.githubusercontent.com/92246505/158686288-9aae4bad-1fba-4d9d-956a-14bd0c9c7261.png">

<img width="960" alt="Deliverable 3 2 2" src="https://user-images.githubusercontent.com/92246505/158686308-50077b1f-0a63-4c3f-888b-3198ed20b7d6.png">


Deliverable 4 - Study Design: MechaCar vs Competition:

For each single measure that may be examined, a unique hypothesis would need to be devised, as well as a statistical test tailored to the exact metric requirements. Metric Criteria That Could Be Used

Data might be obtained from the MechaCar model and compared to a specific competition model based on the criteria listed below.

Acceleration Speed Cost (Selling Price) Fuel Efficiency Comfort (Space & User Functionality)

Null Hypothesis (Ho): When compared to other cars of its sort, the MechaCar is more fuel efficient. Alternative Hypothesis (Ha): The MechaCar is not more fuel efficient than similar cars.

To test the hypothesis, I propose utilising the t-test. I recommend adopting this since there is just one dichotomous independent variable and only one continuous dependent variable. Furthermore, the analytical issue we are posing is whether or not there is a statistical difference in the mean of the two samples. Outline of Statistical Tests

The strength of the connection would be determined using the conventional p-value of 0.05, with a number more than suggesting a lesser degree of significance and bigger values indicating a higher level of significance. Fuel economy would be measured in kilometres per litre (kpl) for both the MechaCar and competition vehicles, with a 60L engine.

