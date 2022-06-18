# CALIFORNIA_WATER_ANALYSIS

An Analysis of California's Groundwater Data
I heard the water levels are dropping in California. I saw this article that there is an ongoing drought in California:
California's water supply goes beyond the current drought
After being repeatedly told to conserve, most Californians realize we have been in a drought for several years and that…www.ocregister.com
So, I got curious about what the water levels are really like. California tracks their water levels in open data online. The data can be found here:
Periodic Groundwater Level Measurements - California Open Data
The DWR Periodic Groundwater Levels dataset contains seasonal and long-term groundwater level measurements collected by…data.ca.gov
I looked at their groundwater measurements for the top 10 wells that are in the area. They have an excel which shows the different columns and their purposes: 
We are going to focus on "GWE" and SITE_CODE which will tell us the ID of the wellWe see here GWE is our main target to measure. It shows the groundwater elevation above sea level. The lower that number, the worse the water situation is. 
I loaded their measurement dataset Let's take a look at a basic EDA of their measurement data:
These reflect the types in their excel sheetThese are the top 10 well IDs with the most measurements. Ripe for our plottingWe also see the different agencies that report about the water levels. The top 10 orgs that reportI'm curious what this unknown means. This is how they measured the water…but why so many unknowns? Did they use a long stick or something?We see that although more than half are voluntaryThe above picture, SGMA stands for the Sustainable Groundwater Management Act.
Sustainable Groundwater Management Act (SGMA)
In 2014, Governor Edmund G. Brown Jr. signed three bills known collectively as the Sustainable Groundwater Management…water.ca.gov
CASGEM stands for California Statewide Groundwater Elevation Monitoring
Groundwater Monitoring (CASGEM)
Since 2009, the California Statewide Groundwater Elevation Monitoring (CASGEM) Program has tracked seasonal and…water.ca.gov
Now, I plot the top 10 measured Wells with their groundwater elevations. Please note that for some of them, they only had limited data, maybe the well shut down. 
The #1 Well that is measured does show some crazy dips recently. Well below the regular lows from the previous years. The 2nd Well however, shows an alright levelThis is a bit alarming. Well #3 has gone below 2019 levels.I wish there was more information on the location of the wells. Definetly something for future work. Some of the wells are spiling in volume and some are staying at the same height.These last two in the top 10 only show limited data. Still, it is cool to see there looks like some seasonalityThoughts/Conclusion/Future Work
There are some wells which show that the groundwater elevation has lowered drastically
There is limited data on some of the wells. For future work, I can limit the data to only the most recent 10 years and repeat the plotting
I want to plot these Well IDs with wherever they are coordinated. I'm curious to see which areas are not affected by drought and where others are affected. 
Based on the data, there are some areas where there is a decrease in groundwater levels. 
What is California doing to solve this problem? It seems they cannot do desalination: https://www.ocregister.com/2022/06/06/water-restrictions-show-folly-of-californias-rejection-of-large-scale-desalination-projects/
