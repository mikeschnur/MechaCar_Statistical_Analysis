# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![Screen Shot 2022-09-26 at 12 06 12 PM](https://user-images.githubusercontent.com/108902185/192327670-7ade53ec-3891-4e4e-b3fd-38930f31ac09.png)
1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
At a 95% confidence level, an alpha of .05 is used to determine whether the p-value is statistically significant or not. 
Coefficents of Variables:
MPG (Intercept) = 0 is less than .05, making MPG statistically significant with a non-random amount of variance
Vehicle Length = 0 is less than .05, making Vehicle Length statistically significant with a non-random amount of variance
Vehicle Weight = .078 is greater than .05, making Vehicle Weight not statistically signifcant with a random amount of variance
Spoiler Angle = .31 is greater than .05, making Spoiler Angle not statistically signifcant with a random amount of variance
Ground Clearance = 0 is less than .05, making Ground Clearance statistically signifcant with a non-random amount of variance
AWD = .19 is greater than .05, making AWD not statistically significant with a random amount of variance

2. Is the slope of the linear model considered to be zero?
The Coefficents for each variable are:
Vehicle Length: 6.267
Vehicle Weight: .001
Spoiler Angle: .069
Ground Clearance: 3.546
AWD: -3.411

The resulting formula for MPG = -.01 + 6.267(Vehicle Length) + .001(Vehicle Weight) + .069(Spoiler Angle)+ 3.546(Ground Clearance)-3.411(AWD). Which yields a non-zero slope. 

3. Does the linear model predict MPG of MechaCar prototypes effectively?
The R-squared value of .7149 shows a moderate to strong correlation for the data, indicating the model to have effectively predicted the MPG of MechaCar prototypes in most cases.

## Summary Statistics on Suspension Coils

# Manufacturing Lot Summary
The summary statistics for the manufacturing lots are displayed below.

![Screen Shot 2022-09-26 at 12 56 06 PM](https://user-images.githubusercontent.com/108902185/192336277-045b0548-c1b1-41b9-a8dd-8bb08e04c6ed.png)

# Manufacturing Lot Summary - By Lot

![Screen Shot 2022-09-26 at 12 57 16 PM](https://user-images.githubusercontent.com/108902185/192336443-5f8ec149-3361-4d3c-b0f1-3c0f6c701679.png)

1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
All of the lots in total meet this threshold with variance of 62. Although Lot 3 had a variance of 170 which is much higher than the limit of 100. Lots 1 and 2 had very small variances of .97 and 7.47 respectively, which explains the overall lot meeting the requirement while the 3rd lot having such a high variance. 

## T-Test on Suspension Coils

#T-test on all Lots

![Screen Shot 2022-09-26 at 1 16 12 PM](https://user-images.githubusercontent.com/108902185/192339792-05a6ef45-a664-4368-832d-8c7012a1dcf0.png)

The p-value of 1 is greater than the alpha of .05. This indicating the total manufacturing lot does not statistically vary from the normal distribution at a significant level with a mean that falls within the confidence interval.

#T-test on Lot 1

![Screen Shot 2022-09-26 at 1 24 02 PM](https://user-images.githubusercontent.com/108902185/192341135-48eb936a-0f22-4d4a-88bf-7f90859f1666.png)

The p-value of 0.0 is less than the alpha of .05. This indicating the total manufacturing lot does statistically vary from the normal distribution at a significant level with a mean that falls within the confidence interval.

#T-test on Lot 2

![Screen Shot 2022-09-26 at 1 26 25 PM](https://user-images.githubusercontent.com/108902185/192341645-c7dbb71f-8b5e-4502-91d9-fa78f6c2df78.png)

The p-value of 0.0 is less than the alpha of .05. This indicating the total manufacturing lot does statistically vary from the normal distribution at a significant level with a mean that falls within the confidence interval.

#T-test on Lot 3

![Screen Shot 2022-09-26 at 1 27 18 PM](https://user-images.githubusercontent.com/108902185/192341819-31f4e187-e211-471c-b802-24442bb5b0e7.png)

The p-value of .1589 is greater than the alpha of .05. This indicating the total manufacturing lot does not statistically vary from the normal distribution at a significant level with a mean that falls within the confidence interval.

##Study Design: MechaCar vs Competition
1. This study would be on the MPG on the highway as well as the city for the MechaCar prototypes versus the Competition.

2. The null hypothesis would be that there is no difference in highway and city MPG for MechaCar vs the Competition. The alternative hypothesis would be that there is a difference in the city and highway MPGs between MechaCar and the Competition.

3. A t-test on the both the highway and city MPGs for MechaCar and the Competition would yield the disired data.

4. A random sample of more than 30 MechaCar and thei competitor's city and highway MPGs would be needed for this testing. 
