# IVP2
DH2321 Information Visualization - Project 2

## Analytical Trail 1

Started at www.worldvaluessurvey.org, searched for countries appearing over all time-periods (wave). I particularly liked the sub-group about children qualities. People are surveyed in multiple countries to determine which qualities are most desired/seen in children during that time-period. 

Once all the data was aggregated in tables. Column headers corresponds to Variables like Country Code (cc), Country Name, Independence, Thrift saving money and things, Unselfishness, Religious, Imagination, Tolerance and respect for other people, Determination, Hard Work and Obedience. The Row headers corresponds to 30 selected countries not arranged in order. 

The data was exported from excel in CSV format and then converted to JSON using online tools. The JSON data is used to generate geomaps in d3.
In addition to d3js, d3Plus.js (d3plus.org) is used to simplify map rendering. Five maps are created ranging from 1989 to 2014, each with 5 year wave. Selected countries are plotted and variable data is shown in tooltips. 

Buttons at bottom allows user to switch between different time-waves and see the data geographically. One can also compare values between two countries in same time-wave by clicking on one country and hovering over the other. 


## Analytical Trail 2

After creating world-maps, the expression of data felt limited by the fact that the world-map is not a good choice to display multiple variables at the same time. A solution was to create multiple combinations of maps (40, crossing 5 time-waves with 8 variables). 

A better solution is to create parallel coordinates. This representation allows for easier and more expressive date visualisation among multiple variables.
Taking inspiration from a Columbia University project, I created a multivariate parallel coordinates chart marking countries, years, and other eight variables. 
Along with data-table connected to the chart, the user has good amount of options for filtering and comparing. 

To filter data, one must drag cursor over any axis. This creates a selection and it filters the data. The filtered data is visible in Data-Table below. Though the data-table is limited to 10 entries, it suffices once filtration begins. 

Hovering over a data-row in Data-table will highlight the plot-line in the chart. Buttons like “Keep”, “Exclude” and “Reset” allows to hold filtered settings for prolonged comparison. 

This visualisation provides a great overview and in-depth knowledge about each value-point.

## Result

The result is a website which presents survey-data about Important Qualities in Children among different countries across span of 25 years. The visualisation is a hybrid of geo-maps and multivariate parallel coordinates chart. The website allows user to switch between them and compare or filter selected variables. 

## Learning

It was clear that map-based visualisation is more attractive feature but the permutations of variables across time made that difficult to achieve. Parallel coordinates solves the problem albeit isn’t as easy to understand. I learnt quite-a-lot while developing this project and in future, maybe I’ll create better visualisations. 
