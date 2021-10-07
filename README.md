# Mecha Car analysis
This analysis is to use R and statistical tests to review car data for a car manufacturer MechaCar.

# Linear regression to predict MPG

![cap5](https://user-images.githubusercontent.com/82550431/136375758-96f6e081-863e-449b-ba3f-78b7941ddc43.png)

For the first analysis, a multiple linear regression is used to see what variables are related to MPG. The variables examined were vehicle length and weight, spoiler angle, ground clearance and All wheel drive. *Results shown above*

Based on the shown data, the intercept, vehicle length and ground clearance g a non-random amount of variance to the MPG values in the given data. The p-value is less than the signifcance level of 0.05, rejecting the hypothesis in regards of the althernative that the slope is not zero. This regression is fairly effecive at predicting the MPG, it accounts for about 70% of mpg value, based on the R-squared value of 0.7149. Although, there is still variation that is not accounted for based on this regression.

# Statistics on suspension coils
The next analysis for the MechaCar was to evaluate the PSI variance of the suspension coils. The design specifications for the MechaCar suspension coils explain that the variance of the suspension coils must not exceed 100 pounds per square inch. This was evaluated by looking at all the data put together, as well as by each lot individually. The summary for the combined data is shown below. This shows an overall variance of 62.2, which is in the 100 PSI limit.

![Cap1](https://user-images.githubusercontent.com/82550431/136377015-998b6ba1-45ab-4f09-a527-7236389d7282.png)

The summary for the lots are shown next below. This shows that Lots 1 and 2 pass the specification, because their variances are less than 100. However, Lot 3 fails to meet the requirements since the variance is 170.

![cap2](https://user-images.githubusercontent.com/82550431/136377032-4062d046-bb48-4ab1-9206-6ce83fb907ea.png)

# T-Test on suspension coils
The third analysis for MechaCar was to look at the average PSI for the suspension coils compared to the required of 1500. This was done by performing a 1 sample t-test with all the lot data grouped, and then 3 additional indivdual sample t-tests to compare each of the lots to the specification. When all lot data was combined, the p-value of the t-test was 0.0603. This is higher than the significance level of .05, so we cannot reject the null hypothesis that the mean is 1500. The t-test results for the combined lot data is shown below.

![prelot](https://user-images.githubusercontent.com/82550431/136378024-32aa155c-82e7-44dc-9e08-fbd10b1827c6.png)

 
Lots 1 and 2 have a p-value higher than the significance level (1 and 0.6072), so we cannot reject the null hypothesis. Although, Lot 3 has a p-value of .0417, lower than the significance level, which means to reject the null hypothesis and alternatively that the mean does not equal 1500. So while the combined lots meet the specification, lot 3 does not meet the criteria. 
The results for the individual lots are shown below.


**Lot1**

![lot1](https://user-images.githubusercontent.com/82550431/136378040-5a536d9d-9ae0-4dac-8ec9-e8c741b97ada.png)

**Lot 2**

![lot2](https://user-images.githubusercontent.com/82550431/136378064-5ed50bcf-4bc8-4e20-9f4a-4129c3abc0e5.png)

**Lot 3**

![lot3](https://user-images.githubusercontent.com/82550431/136378078-f88307c5-bacf-41c8-ac0c-3f0f2bf0b252.png)
