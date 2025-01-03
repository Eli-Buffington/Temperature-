---
layout: default
---
<h1>Correlation between Carbon Dioxide Emissions and Temperature in the United States</h1>


## Analysis By Cameron Hendry and Eli Buffington

# Introduction

Climate change has irrefutable evidence for its existence. The research has been conducted on datasets going back hundreds of years, showing an increase in the global temperature that is undeniable, giving the length and accuracy of the data. But the relatively lax carbon dioxide regulations and tracking, where corporations have every economic desire to try to circumvent, are much of what is reported when it comes to carbon dioxide emissions. Do these guidelines help predict the change in temperature? If so, how long before the effects are statistically significant, as climate is notoriously unpredictable past a few days. 
Is there a correlation between a change in carbon dioxide emissions and a change in  Temperature? We suspect a correlation because of a multitude of peer reviewed studies on the effect of greenhouse gasses and climate change, but would a statistically significant correlation show up in the relatively short 25-30 years of our data? 
 The data that we used was temperature data from the United States and carbon dioxide data from the United States from 1991 to 2019. These were two separate datasets, which were merged together for further analysis. The data was from reputable sources and thus was very easy to process, leading to few issues with the data. Downloading the data was made simple by the websites allowing a choice between different time periods and sample frequencies. The only slight hurtle was lining up the data and merging the two dataframes together, as the columns, while both being a date, were formatted differently, leading to significant reprocessing before merging. 

We graphed the merged data frame on the same graph and attempted to line the effects of carbon dioxide emissions up with a corresponding effect on temperature. We then regressed the change in carbon dioxide emissions on the change in temperature, both shifted and unshifted, to find the correlation between these two datasets by obtaining a p-value and a line of best fit. 


# Methods & Results

We compared these two time series datasets by merging the two separate data frames together on the time column. We only used yearly data averaged on January 1st of every year. One of the bigger issues that came up was how to plot data with two different units on the same graph. The way we solved this is by having two different y-axes, one on the left and one on the right side of the graph, so that we could see both graphs together on the same chart. 


{% include_relative fig1.html %}

The above is change in degrees celsius and change in tons of carbon dioxide emissions plotted on the same graph. We observed that a change in carbon dioxide emissions is followed by a change in temperature after two to five years. This is reasonable because climate change is a slow process that happens over years not months or days. Carbon dioxide  emitted from someone’s tailpipe probably does not instantly affect the temperature which explains the lag in the data. 


We used this data to run a linear regression on change in degrees celsius and change in tons of carbon dioxide emissions, with change in tons of carbon dioxide emissions as our independent variable and change in degrees celsius as the dependent variable. The regression had an R<sup>2</sup> of 0.024, which means that only 2.4% of the change in temperature was explained by a change in carbon dioxide emissions. The regression equation is displayed on the following graph. The p-value on the coefficient on change in tons of carbon dioxide emissions was 0.421, which is far above the statistically significant value of 0.05. This means that we cannot reject the null and we cannot conclude that the effects were anything but chance. 


{% include_relative fig2.html %}

This is a graph with difference in yearly carbon dioxide emissions as the independent variable and difference in yearly temperature as the dependent variable, with the line of best fit plotted over the data points. This graph explains our low p-value, as our data does not follow the line. Additionally, the slope of the line is negative, which implies that increasing carbon dioxide dioxide correlates with a decrease in temperature, which is illogical.

We then shifted the data for temperature by ten years in either direction and calculated the correlation coefficient for each. We then took the highest one and shifted our data by that amount. In our case, we concluded the offset was -5, meaning that the change in carbon dioxide emissions was most correlated to temperature changes in 5 years. 

{% include_relative fig3.html %}

In the above graph we shifted the temperature graph by 5 years to showcase how the delay lines up and dropped 5 years off the end of both graphs. This graph shows how the CO2 emissions would affect the temperature if the effects were instantaneous. A bunch of the peaks and valleys line up pretty perfectly near the beginning and for some reason near the end there is less correlation which we are still unable to explain. 


We used this shifted data to run a linear regression on change in degrees celsius after the shift and change in tons of carbon dioxide emissions, with change in tons of carbon dioxide emissions as our independent variable and shifted change in degrees celsius as the dependent variable. The regression had an R2 of 0.069, which means that only 6.9% of the change in temperature was explained by a change in carbon dioxide emissions. The regression equation is displayed on the following graph. The p-value on the coefficient on change in tons of carbon dioxide emissions was 0.216, which is far above the statistically significant value of 0.05. This means that we cannot reject the null and we cannot conclude that the effects were anything but chance. 

{% include_relative fig4.html %}

This is a graph with the difference in yearly carbon dioxide emissions as the independent variable and the shifted difference in yearly temperature as the dependent variable, with the line of best fit plotted over the data points. This graph explains our medium p-value, as our data does not follow the line well but there appears to be some sort of collocation which explains our lower p-value, although not enough to be statistically significant. Additionally, the slope of the line is positive, which implies that increasing carbon dioxide dioxide correlates with an increase in temperature, which shows that this is likely closer to the truth than the previous analysis.


# Conclusions

Unfortunately, we were unable to find a statistically significant p-value, even after shifting the data to account for any lags between when the carbon dioxide  was produced and when the temperature changed. We were unable to reject the null hypothesis, which was that a change in carbon dioxide release has no effect on change in temperature. A major limitation to our data is that it only accounted for United States temperature and carbon dioxide  emissions and was blind to less local effects. Another limitation was that the tracking of carbon dioxide  emissions in our publicly available data set only went back until 1990, so we were unable to observe longer term changes that might have yielded more significant results. We believe that the magnitude of climate change was low enough across the relatively short chunk of time we measured that our analysis was blind to its effects, and was masked by the local unpredictability of climate. We would not recommend making long term conclusions based on our failure to reject the null hypothesis. 
An area for future study would be looking at atmospheric carbon dioxide emissions instead of carbon dioxide release. This would yield greater insight into the effects of carbon dioxide emissions as it would bypass the country specific reporting requirements that are prone to corruption and the falsification of results. 
