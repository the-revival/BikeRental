# BikeRental
> The project aims to predict demand for shared rental bikes based on some parameters.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- The project aims to predict demand for shared rental bikes based on some parameters.
- Background: A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
- BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.
- Dataset: http://dx.doi.org/10.1007/s13748-013-0040-3

## Conclusions
- The demand peaks during summer and fall and then gradually decreases during the winter to the lowest during spring.
- Whether it's a working day or not doesn't have a great impact on the median demand. The spread during non working days is greater than on weorking days with the lower hinge
being lower than the working days and upper hinge being almost the same.
- The demand decreases when the weather is misty or rainy. The dataset had no data points during heavy rain. So, predictions during heavy rain cannot be made.
- The demand increases from 2018 to 2019 with lower hinge, median and upper hinge for 2019 being higher than those of 2018. This suggests that the demand is increasing year on year.
- Since the feeling temperature combines the temperature, humidity and windspeed, so it is used as a proxy for these.
- Since working day is closely related to holidays and days of the week, working day is considered instead of holidays and days of the week.
- Since season changes with the month and the demand is dependednt on season, month is not taken into consideration in the final model.
- Registered users have a higher ratio than casual users in the total demand. But, since the number of registered users is not given in the model, it cannot be used as a predictor.
- The final model has the following parameters: atemp, fall, spring, summer, LightRain, Mist. All of the predictors have a low VIF and p-value.
- The R-squared value on the final model: 0.805, adjusted r-qquared: 0.802, F-statistic: 296.4. So, the model has a good R-squared and is significant.
- The R-squared value on the test data set: 0.804. So, the model is able to generalize well to the test dataset.

## Technologies Used
- numpy
- pandas
- matplotlib
- seaborn
- statsmodels
- sklearn

## Contact
Created by [@the-revival] - feel free to contact me!