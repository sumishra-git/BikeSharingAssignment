# BoomBikes Bike Sharing Assignment

## **Problem Statement**

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider **BoomBikes** has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands <br>

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

**Business Goal**:

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Recommendations](#recommendations)
- [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

**Issues to Address:**

1. **Revenue Decline:** BoomBikes faces substantial revenue declines due to the ongoing pandemic, necessitating a strategic solution.
2. **Market Sustainability:** The company struggles to sustain itself in the current market scenario, demanding a mindful business plan.
3. **Post-Lockdown Strategy:** BoomBikes aims to accelerate revenue post-lockdown, requiring an understanding of post-quarantine bike demand.

**Objectives:**
The objectives include predicting significant variables influencing American market shared bike demand, determining the crucial predictors, developing a model to understand demand variations, facilitating adaptive business strategies, and exploring demand dynamics for effective decision-making. This case study aims to achieve this goal by building a multivariate linear regression model using the provided [dataset](./day.csv).

The primary objective is to identify the key variables that significantly influence the prediction of shared bike demand and assess how effectively these variables describe the patterns in bike demands.

## Conclusions

- The close alignment of R2 score between the training and test sets (0.78 vs 0.75) in a linear regression model indicates effective generalization. This similarity suggests the model avoids overfitting to the training data and is likely to perform consistently on new, unseen data.
- The RMSE values of 822903 in the training set and 911580 in the test set for a linear regression model indicate that the model is fitting well to the training data and generalizing reasonably to new, unseen data with a small difference between training and test set performance.

Significant variables to predict the demand for shared bikes:

- Year 2019 has higher bookings compared to year 2018, means the bookings are increasing year on year and company can predict higher booking for upcoming year.
- The demand also increases with temperature (clear weather) and decreases for cloudy weather and highly decrease for bad weather condition with high windspeed, hence it should keep track of the weather conditions.
- Holiday time has least bookings whereas most working days and even weekends has a positive demand. Suprisingly, Mondays have less bookings which could be because of hybrid work culture where most companies are work from home on Mondays.
- The month September and october (Fall season) should be considered by the company as they have a higher demand, this could be because of mostly clear weather condition. And Month January and February (Winter season) has negative impact on bookings which could be due to the severe weather conditions like snow and low temperature. Also July has less bookings which could be due to rainfall and cloudy weather condition.

## Recommendations

- **Leverage High-Impact Features:** Focus on features such as **temp**, **yr**, and **Winter** as they exhibit the highest coefficient values, indicating significant impact on bike demand.

- **Seasonal Strategies:** Develop targeted marketing and pricing strategies for different seasons, particularly emphasizing promotions during **Winter**.

- **Weather-Sensitive Promotions:** Implement weather-specific promotions or incentives to encourage bike usage during favorable weather conditions, addressing the impact of **temp**, **hum**, and **windspeed**.

- **New Market Insights:** Use the developed model to gain insights into demand dynamics in the American market, informing business strategies and positioning BoomBikes competitively.


## Technologies Used

- [Python](https://www.python.org/) 
- [Matplotlib](https://matplotlib.org/) 
- [Numpy](https://numpy.org/) 
- [Pandas](https://pandas.pydata.org/) 
- [Seaborn](https://seaborn.pydata.org/) 
- [Statsmodels](https://www.statsmodels.org/stable/index.html) 
- [Scikit-Learn](https://scikit-learn.org/stable/) 

## Acknowledgements

- This project was inspired by upGrad on Industry Relevance of Linear Regression Models by [Susmita Mishra]
- UpGrad tutorials on Linear Regression on the learning platform

## Contact

Created by [@sumishra](https://github.com/sumishra-git)