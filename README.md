# Project Name : Bike sharing Assignment
> Bike sharing Assignment

**Problem Statement**
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

the variables are significant in predicting the demand for shared bikes. and how well those variables describe the bike demands Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.


## Table of Contents
 **Step 1: Reading and Understanding the Data** .
 **Step 2: Visualising the Data**.
 **Step 3: Data Preparation**
**Step 4: Splitting the Data into Training and Testing Sets**
**Step 5 :Rescaling the Features**
**Step 6: Building a linear model**
	Model 1:Building model using statsmodel, for the detailed statistics
	Model 2:Removing the variable 'hum' based on its High VIF
	Model 3:Removing the variable "workingday" based on its Very High 'VIF' value. Even though the VIF of workingday is second highest, we decided to drop 'Workingday' and not 'temp' 
          based on general knowledge that temperature can be an important factor for a business like bike rentals, and wanted to retain 'temp'. 
	Model 4:Removing the variable "weekday_Saturday" based on its Very High 'P' value. Even though the VIF of workingday is second highest, we decided to drop 'Workingday' and not 'temp' based on general knowledge that temperature can be an important factor for a business like bike rentals, and wanted to 	retain 'temp'

**Step 7: Residual Analysis of the train data**	   In order to check if the error terms are also normally distributed (which is infact, one of the major 	   assumptions of linear regression), let us plot the histogram of the error terms and see what it looks like.

**Step 7: Making Predictions Using the Final Model**

**Step 8: Model Evaluation**	

### Conclusion : 

We can cosider the above model i.e lr4, as it seems to have very low multicolinearity between the predictors and the p-values for all the predictors seems to be significant.

F-Statistics value of 213.1 and the p-value of 3.97e-187 i.e almost equals to zero, states that the overall model is significant

Hence, we finalise lr_4 as the final model to proceed with the future predictions.

### Final Conclusions : 
By using the above scatter plot and the table , We can see that the equation of our best fitted line is:

cnt =0.12155 + (0.2342year) −(0.0973holiday) + (0.4728temp) − (0.1549windspeed) + (0.0762mnth_sep) + (−0.2864weathersit_Light Snow & Rain) + (-0.0807×weathersit_Mist & Cloudy) + (−0.0615×season_Spring) + (0.0422×season_Summer) + (0.0771×season_Winter)
All the positive coefficients like temp,season_Summer and season_W𝑖𝑛𝑡𝑒𝑟 indicate that an increase in these values will lead to an increase in the value of cnt.

All the negative coefficients indicate that an increase in these values will lead to a decrease in the value of cnt.

From R-Sqaured and adj R-Sqaured value of both train and test dataset we could conclude that the above variables can well explain more than 81% of bike demand.

Coefficients of the variables explains the factors effecting the bike demand

Based on final model top three features contributing significantly towards explaining the demand are:

Temperature (0.4728)

year (0.234287)

weathersit_Light Snow & Rain (−0.2864)

Hence, it can be clearly concluded that the variables year, temperature , and weathersit are significant in predicting the demand for shared bikes .

## Final Recommendations for the Company:

The months - Jan , Jul , Sep , Nov , Dec should be considered by the company as they have a higher demand as compared to other months. With an increase in temperature the demand also increases, hence it should keep track of the weather conditions. During the Winter season the demand rises, hence it should be well prepared to meet the high demand.


## Contact
Created by [https://github.com/Rakesh-Rangadal] - feel free to contact me!

