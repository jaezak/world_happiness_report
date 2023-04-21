Introduction

Presentation is included in the main repository and is also available at this link to Google Slides:
https://docs.google.com/presentation/d/1bmeHbTOph0_ZMg_E_6G9Ibjx0hwqrrj_z0xc9wNeAJ8/edit?usp=sharing

The World Happiness Report takes data from the Gallup World Poll surveys and formulates them into what is called the Cantril Self-Anchoring Striving Scale, or the Cantril Ladder. Developed by Dr. Hadley Cantril in 1965, it asks respondents to imagine a ladder with steps numbered from zero at the bottom to 10 at the top.


The top of the ladder represents the best possible life for you and the bottom represents the worst possible life. Pollers are then asked which step of the ladder they feel they are on.
"Thriving" respondents had ratings of 7 or higher and reported significantly fewer health problems, less stress and anger.
Ratings of 5-6 categorized as "Struggling", with more daily stress and worries about money than "Thriving" respondents. 
Ratings of 4 and below fall into the "Suffering" category, where well-being is at high risk, and usually report lacking basic needs such as food and shelter, and less access to healthcare.
The World Happiness Index suggests 6 key leading indicators for happiness:  income, healthy life expectancy, having someone to count on in times of trouble, generosity, freedom, and trust (measured by the absence of corruption in business and government).
Data Resource and Programs Used
We sourced our data from a dataset found on kaggle.com composed of the World Happiness Reports for 2015-2021. We decided to omit the 2020 and 2021 datasets because we did not want to take the COVID-19 pandemic into consideration in our findings. Programs used for data analysis include Python Pandas, MatplotLib, and SciPy.
Trust in Government
American Economist and co-editor of the WHR Jeffrey Sachs said,
"The lesson of the World Happiness Report over the years is that social support, generosity to one another, and honesty in government are crucial for well-being. World leaders should take heed. Politics should be directed as the great sages long ago insisted: to the well-being of the people, not the power of the rulers.”
Testing for correlation of trust in government and happiness was measured in 5 scatter plots for each year's dataset. Linear regression and the r-squared value was calculated, as well. The r-squared values for each year were quite low, (an average of .16) , which is to be expected considering the concept of trust is subjective. R-squared values tend to be quite low in the field of social science because human behavior can be very unpredictable. The data indicates a weak correlation between perception of corruption and happiness and there is no incentive to further investigate this data.
There has been a broad range of studies showing that communities with high levels of trust are generally much more resilient in the face of a wide range of crises, including natural disasters, war, and civil unrest. According to the World Happiness Report Website:
“Trust and cooperative social norms not only facilitate rapid and cooperative responses, which themselves improve the happiness of citizens, but also demonstrate to people the extent to which others are prepared to do benevolent acts for them and for the community in general.”
Including datasets for the years 2020, 2021, 2022, and 2023 could potentially show a stronger correlation between the two variables when monumental political events/crises such as the 2020 US Presidential election, COVID-19 pandemic and the war in Ukraine occuring during this time period.
Economy (GDP per Capita)
According to the World Happiness Report, the statistics of GDP per capita (variable name gdp)  are also considering purchasing power parity for all countries surveyed where there was available data based on each year. This was pulled from the World Bank Open Data, and the researchers have an interpolation and extrapolation method to fill in the missing years.
Generally, we assume that living in a richer country means a more secure, comfortable, and overall happier life. We have historically measured a nation’s success based on their total GDP. The methods for categorizing developed nations is mainly based on poverty and the economy. Countries with a very high GDP will have a population with greater individual incomes and overall individual wealth. Money can buy happiness, to some extent. 
After analyzing our data, we saw positive relationships between GDP per Capita and the Happiness score for different countries. There are graphs for scatter plots relating those two factors in 2015 - 2019. Over time, the R-squared value of the relationship between overall Happiness Score and GDP per Capita shows a moderate to strong correlation since R-squared ranges between 0.61 - 0.66. In the normal distribution histograms, there’s a slight skew to the right which indicates there are more countries with a higher GDP per capita and higher happiness score than there are with lower GDP per capita and lower happiness score. 
Healthy Life Expectancy

Average number of years that a person can expect to live in "full health" by taking into account years lived in less than full health due to disease and/or injury, measured with both physical and mental conditions
Q: What is the metric of this variable? - From score 0 to 1+, what range should be considered GOOD, what range should be considered BAD?
Q: What ranges do the Top & Bottom 5 countries (2015-2019) land in? - In this variable, are top happy countries all in the GOOD categories, and bottom happy counties all in the BAD categories throughout the years?
Collect HALE (Healthy Life Expectancy) scores of all participating countries in all 5 years. 
Get the statistic UPPER QUARTILE (Q3,75%) as the critical value for the GOOD category.
Vice versa, get the statistic LOWER QUARTILE (Q1,25%) as the critical value for the BAD category.  
Evaluation of the Top 5 Countries | 2015-2019
7 countries have been in the Top 5 from 2015-2019
Norway and Denmark - ever fall off the GOOD category
2016 & 2017 vs. 2019
Evaluation of the Bottom 5 Countries | 2015-2019
10 countries have been in the Bottom 5 from 2015-2019
Syria, Rwanda and Tanzania - ever above the BAD category
2018 vs. 2019
Family

When analyzing Family in comparison to the happiness score we wanted to make a scatter plot year over year to see if there was a difference that could have occurred. 

And saw that they looked to be pretty consistent with an average r-squared value below .58 which suggests that there is moderate to strong relationship between the two with an r-squared value of .604 in 2019 to give us even more confidence to see how normally distributed the data looks to be.

Sadly the normal distribution year over year looks to be skewed left, giving us reason to believe that family is an important factor when measuring happiness score. We find this to be interesting as family can definitely act as a rock when going through tough times. We do however believe that family should not be the most important factor as there are other variables that contribute to happiness.

To further prove that family is important when measuring the happiness score we wanted to measure the mean score between the top 5 and bottom 5 and found that the mean score amongst the top 5 countries is 1.44 and for the bottom 5 it was .47. The data didn't give context as to the upper and lower bound so we went with anything above a 1 is considered good and vice versa for anything below one. But it's clear to see that the difference between the two is far and can give insights into how the extremes can give validation to family being an important factor.
Freedom

When looking at freedom I was surprised to see that the r-squared was incredibly weak by having a score of .31 suggesting that the relationship wasn't strong enough to go into further analysis as freedom seems a bit broad. And as you can see the scatter plot is all over the place thus proving it difficult to draw any analysis from it.


Generosity

When it came to  generosity we were surprised to see it be normally distributed between the years 2015-2017 and straying from a normal distribution between 2018-2019 thus prompting us to look at a scatter plot to see its relationship to family score.

And by looking at the scatter plot most of the values tend to group in the bottom but still appear to be random. The r-squared was .321 which is similar to freedom and gives us the same outcome of not digging deeper as we have low confidence in the relationship. 
