# fp-Evelyn-Valerie

**Homicides in Mexico: 2006 to 2015**

## Please find the link to the dashboard here:



# Introduction

In 2011 Mexico got under the international spotlight for an unprecedented phenomenon: the brutal increase in violence, especially reflected in the rise of homicides. Its geographical distribution has changed over the years, reflecting the government strategies and the interaction of criminal groups.

The propose of this project has disintegrated these phenomena for a better understanding, focusing on the chronology and spatial distribution of the homicides during 2006 to 2015. Additionally, we include a special section related to gender homicides, that have been increasing in Mexico. Finally, we include an interactive visualization, focus on creating a conscious among our target audience, by providing information of how this wave of homicides affected people with the same socio-demographic characteristics.

*Data

The database used in our analysis was provided by Data Civica and is available to the public at https://www.dropbox.com/sh/99n9h6zjasa6fdr/AAAIkr8aERhNMg-aT8IENqCoa?dl=0

*Methods

For this project we use the following visualization elements:

Interactive graphs: created with ggplotly to provide detailed information about the rate and number of homicides per year. We use column bars and line bars, as well as faced by year. Additionally, we use the tool “crosstalk” that was helpful for the brushing and filtering of the homicide rate of the 32 states and constructed an interactive visualization that allows the user to see the trend of one state individually or compare trends between states, assigning one color to states to facilitate the comparison.

Interactive maps : due to the spatial distribution of the homicides, we constructed three interactive maps merging data with polygon layers, with data from 2006, 2011 and 2015. Additionally, the interactivity makes possible for the user to identify the states are even when it has not strong background in Mexican geography since the interactive map shows the name of the states.

Visualization: to support our platform, we use a flex dashboard, adding multiple elements, such as multiple pages, storyboard and value boxes to make facilitate the narrative of the project and to highlight the most important elements.

Shiny app: we created an app to involve the user with the phenomena of violence, by providing information of the total number of victims within this period that has the same socio-demographic characteristics, such as age, state of residence, level of education and gender.

*Conclusion

We believe the addition of graph and interactive elements to explain the evolution of homicides was fundamental. Geographic and temporal characteristic in a static visualization makes that the reader have to do an extra effort to estimate the values in the trends and also require to have a background on the localization of the states to fully understand the message. This information can be shared with a broader audience to have a clear idea about homicides in Mexico. Additionally, with more information on characteristics related to homicides, it will be possible to increase the explanatory power of this dashboard and shiny application.

 #Required libraries in R:

Library(raster)
library(sp)
library(rgdal)
library(readr)
library(tidyverse)
library(crosstalk)
library (plotly)
library(dplyr)
library(ggplot2)
library(rasterVis)
library(doBy)
library(sp)
library(maptools)
library(forcats)
library(ggmap)
library(viridis)
library(stringi)
library(flexdashboard)
library(shiny)
