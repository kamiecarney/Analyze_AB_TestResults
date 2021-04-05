# A/B Tests for E-Commerce Website
## by Kamie Carney


## Dataset

> For this project, I used Python to understand the results of an A/B test run by an e-commerce website. Once the single duplicated user_id row and the rows containing data where the landing_page and group did not match were removed, there were 290,585 data points. With a null hypothesis stating that the new webpage would not have an affect on conversion rate, the data was analyzed with both descriptive statistics and logistic regression analysis.

> Both files were obtained from Udacity and are included: ab_data.csv and countries.csv.


## Summary of Findings

> The overall coversion rate of the population data was .1195. When the data was filtered by "group" categories, the control group had a population conversion rate of .1203 and the treatment group had a population conversion rate of .1188. Which initially suggested that the null hypothesis would not be rejected.

> The A/B test, showed that when the sampling distribution was simulated, the resulting distribution was normally distributed as would be expected. Furthermore, the actual difference in the population conversion rates betwen the new page and the old page fell within the simulated distribution. In addition, the calculated p-value of .905 was very high which continues to suggest that we should not move away from the null hypothesis. This was also confirmed by using the built in z-test function.

> Finally, logistic regression was performed with various variables. First we checked to see if there was a significant difference in conversion based on which page a customer receives. There was no statistically significant evidence that page affected conversion rates. Then I ran a logistic regression test to see what affect country in addition to the page would have on the conversion rate. Again none of the results were statistically significant, although the UK came the closest. Finally, I added the interaction between page and country to the model and none of those results were statistically significant either.

### Conclusion
> After all the testing and descriptive statistics were completed, there was no variable that had a statistically significant effect on conversion rates. Therefore, we fail to reject the null hypothesis and will choose to keep the old webpage.