# Midterm 

## Emily DiPressi and Tiffany Feng 

## Updated Proposal 


## Topic: Inefficient Government Spending on Children and Crime

## Research Question
In today’s political climate, the effects of government policies are more important than ever. In our analysis, we hope to shed light on possible changes to implement in order to promote public good. Does inefficient government spending on children lead to higher rates of hate crime in the United States?

## Importance
If we are able to find a correlation between government spending on children and crime in the nation, we can use this research to better inform government spending and to advocate for changes.

## Spatial Scope
The spatial scope of our project is the United States (broken down by state). We decided on this spatial scope due to the geo data available to us in our datasets. Spatial scope matters in our project because government spending in the US is often depicted by state.

## Data Sources
Our first dataset is on [hate crimes](https://github.com/fivethirtyeight/data/tree/master/hate-crimes). This dataset has information on hate crimes per 100,000, ranging from 2009-2016. Also included is information on the population: unemployment, citizenship, poverty levels, all broken down by state in the U.S. Our second dataset focuses on [government spending in the U.S. on kids](https://github.com/rfordatascience/tidytuesday/tree/master/data/2020/2020-09-15). The data was collected from 1997-2016. It is a state by state breakdown of spending on education, income security, and health on children. The data, specifically, is broken down by state, year, and dollar amount spent. Inflation is accounted for in calculating spend.
In addition, to the datasets above, we also utilized census data in order to obtain geographic information. The population and geoJSON file is from [censusreporter.org](https://censusreporter.org/), specifically the [Total Population table](https://censusreporter.org/data/table/?table=B01003&geo_ids=01000US,040|01000US&primary_geo_id=01000US).
Intended Analysis and Resulting Visualizations
Our project will be analyzing data at the state level in the United States. We plan to create choropleth maps of the US states based on our data on government spending on kids and hate crimes to see if there is any relationship between the two. In addition to disaggregating our data by state, we plan to also visualize our data by creating line graphs and bar charts to find trends among our data over time or regions that we can investigate further.
## Methods

To answer our research question, we split up the datasets and each explored one of the two. We each constructed choropleth maps as well as charts. In order to give the maps a 'geography' column, we merged our datasets with Census data. 

Emily analyzed the Hate Crime data, which was imported as a Panda and merged with racial census data for the geometry aspect. Map visualizations in Matplotlib were first made, to express both the median household income and average hate crime data across the United States. Matplotlib was also used to initially make histograms and bar graphs of this data as well, but the state names for each value were not showing up across the x-axis, so the readability was not ideal. Plotly Express was then used to create the histogram visualizations. With ‘state’ on the x-axis, the graphs are easier to read and understand. This clearly shows all of the states’ values for each income and hate crime rate. Finally, a histogram that combined the hate crime and income values were plotted together, to easily compare the two values against the other per state. 

Tiffany analyzed the US Spending on Kids data, which was merged with Census state population data in order to obtain geometry information. To construct the visualizations, Plotly Express was used. Pandas was also required to wrangle the data and process it for analysis. Tiffany created stacked bar charts of spending in each state per child for the different spending categories. Since there were many spending categories, another stacked barchart of a smaller subset of categories was also created. This was charted over several years (1997 to 2016) in order to analyze changes in spending over time. In addition to stacked bar charts, choropleth maps were also utilized to analyze the spending data. An interactive map with a slider for year was created to visualize spending patterns across states for elementary and secondary education. The same was done to map out US spending on higher education across states.
Expectations for Research Insights
Through our research, we hope to see if there is a relationship between US state-by-state government spending on youth and hate crimes in the country. Through our analysis, we have discovered a few states that have high rates of crime and/or government spending on children, which we plan to investigate further in the coming weeks.

## Findings 
The hate crime data had a few key pieces of interesting outputs. I was looking for states that either stood out for one of the variables or correlated with each of the hate crime averages and median income. The District of Columbia was a standout in the average hate crime data, as it was more than two times the value of the next highest value for average hate crimes.  Mississippi also seemed like it would be a notable state as it had the lowest average income, but it also had a low rate of hate crime. Michigan and North Dakota also seem to be two other states to look into over, as they both had relatively low incomes and high crime rates.  

Elementary and secondary education spending seems to steadily increase over the years from 1997 to 2016. Higher education spending seems to increase slightly from 1997-2016.
But, US spending on education in general seems to plateau from 2009 to 2016. This may be related to the 2008 recession.

For elementary and secondary education spending per child averaged over 1997 to 2016, the top 5 states are District of Columbia, New York, New Jersey, Alaska, and Vermont. When analyzing higher education spending per state averaged over 1997 to 2016, the top 5 states that the US spends the most per child is Wyoming, New Mexico, Alaska, North Dakota, and Hawaii.

## Conclusions
Through the analysis of our data, we found that the District of Columbia stood out due to its high hate crime rate and high spending on elementary and secondary education per child. North Dakota also stood out due to its low income, high crime rate, and high level of spending on higher education per child. 

Our findings for these two states were very surprising and seem to indicate that spending more on education leads to higher hate crime rates. We plan to investigate this relationship further to see if the two are correlated.
 
 
 

