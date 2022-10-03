# Linear-Regression-Project
## Statistical Data Analysis of Alcohol Consumption &amp; Life Expectancy Data
The objective of this project is to determine if there is a correlation between per capita alcohol consumption in Europe and two variables: a country’s GDP growth (% annual) and life expectancy. We all have heard anecdotally that alcohol negatively impacts health, and our assumption is that this relationship would appear in life expectancy data. According to the World Health Organization, alcohol consumption is a causal factor in more than 200 disease and injury conditions. It is estimated that 3 million deaths result from the harmful use of alcohol every year (World Health Organization, 2008). To test multivariable modelling, an additional parameter was selected that could potentially impact life expectancy and alcohol consumption, GDP growth to include in analysis.
The original objective of analysis was to understand the interactions between GDP growth, life expectancy and alcohol consumption. Initial prediction was that alcohol consumption would negatively impact life expectancy and that GDP growth would positively impact alcohol consumption. Therefore to complete data analysis, alcohol, life expectancy and GDP growth datasets were downloaded by country and linear regression analysis in Python was performed.

Through analysis, we arrived at the conclusion that our variables involve multiple and complex causations. This analysis indicates that GDP growth is not a confounder for the dataset reviewed. It concludes that the relation among our variables follow a chain pattern. In Structural Causal Model, Y = Life Expectancy, X = GDP Growth & Z = Wine Consumption

<ul>
    <li>●	𝑍 and 𝑌 are dependent. The higher the wine consumption, the lower the life expectancy.</li>
    <li>●	X and Y are dependent. The higher the GDP growth, the lower the life expectancy</li>
    <li>●	X and Z are likely dependent. GDP growth should result in lower wine consumption.</li>
    <li>●	Z and X are independent, conditional on Y. If we already know the life expectancy, then also knowing the GDP growth shouldn’t give us any better idea of the wine consumption.</li>
</ul>
The output of OLS modelling showed wine consumption has a negative correlation with life expectancy, meaning that as wine consumption increases, there is a decrease in life expectancy. GDP growth has a negative correlation with life expectancy, meaning that as GDP growth increases, life expectancy decreases. This relationship is unexpected, but the weakness of our model (R-squared value of 0.187) tells us that a change in GDP growth does not always result in an impact to life expectancy. GDP growth also has a positive correlation with wine consumption, meaning that as GDP increases, wine consumption increases.            

Several different hypotheses were tested to arrive at this conclusion. Through analysis, it was found that wine consumption is an endogenous variable. Potential exogenous variables that were not analyzed as part of this analysis, that could be explored to uncover stronger correlations include:
●	Alcohol consumption among individuals aged 0-14 (alcohol consumption data captures age 15+ and life expectancy data is from at birth)
●	Sub-regional analysis of alcohol consumption, GDP growth and life expectancy (country or geographic region within Europe)
●	Income inequality, with respect to population.
 

