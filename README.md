# Project4
Shared Colab Link:
https://colab.research.google.com/github/Branth1/Project3/blob/master/Project3.ipynb

GitHub Link:
https://github.com/Branth1/Project4
## Description

This is a study of the data collected by the United States Geological Survey group (USGS) from January 01, 2010 through February 22, 2020. All seismic data being observed has been filtered with a minimum magnitude of 2.5. 

The USGS collects a wide range of data on earthquakes, faults and crustal deformation to increase our understanding of earthquake source processes, occurrence, and effects; and synthesize this knowledge into probabilistic seismic hazard assessments, aftershock forecasts, and ground-shaking scenarios for anticipated major earthquakes.

The data sets being studied and compared are the magnitudes compared to time and location. The following analysis will look at the data from first a wide range Pacific Ocean view coordinate with a coordinate window:

longitude range (-152.93 to -115.66) and latitude range (33.45 to 56.47).

This is followed by a focus on the affects measured in April 2015 and concluded with a focus on the divergent and transform tendencies as seen around the Juan De Fuca Plate. This coordinate window is:

longitude range (-135 to -115) and latitude range (40 to 55).

For a closer look at the work being conducted by the USGS or for further information, their website can be found in the reference section below.
## Background

**The questions we are looking to solve are as follows:**

        1-Across what geographic area are we able to observe earthquake data in the map?

        2-Why are most of the earthquakes in that area?

        3-What is the range and magnitude of the earthquake size in this area?

        4-Where are earthquakes located in April 2015 and what event can be linked to these? 

        5-What patterns are observed in magnitude and location over time for a transform and divergent boundary region?

**The Data used for analysis is:**

Initial Bulk Data set:

https://earthquake.usgs.gov/fdsnws/event/1/query.csv?starttime=2010-01-01%2000:00:00&endtime=2020-02-22%2023:59:59&maxlatitude=56.472&minlatitude=33.445&maxlongitude=-115.664&minlongitude=-152.93&minmagnitude=2.5&orderby=time

Refined Juan De Fuca Plate Data set:

https://earthquake.usgs.gov/fdsnws/event/1/query.csv?starttime=2010-01-01%2000:00:00&endtime=2020-02-22%2023:59:59&maxlatitude=55&minlatitude=40&maxlongitude=-115&minlongitude=-135&minmagnitude=2.5&orderby=time

All Data Was Collected Between Jan 01, 2010 and Feb 22, 2020

For additional information on the analysis used please see the link to the code above.

## Solution/Results

The data was analyzed utilizing the code found in the link above. First the bulk data set was requested, and the magnitude was plotted against time.

**Initial Data Analysis**

Note: For the following graphs, a screen shot is shown. To view the interactive map please visit the link to the colab page above. In all maps, the magnitude of earthquake is referenced by the size of the marker.

**Bulk Data Scatter Plot**

![](https://github.com/Branth1/Project3/blob/master/Bulk%20Scatter.png?raw=true)

**Bulk Data Map**

![](https://github.com/Branth1/Project3/blob/master/Bulk%20Map.png?raw=true)

**Interactive Map**

Note: In the live version, the years visible can be filtered by clicking on the legend. Hovering over the indicator will display the coordinates, date and magnitude.

![](https://github.com/Branth1/Project3/blob/master/Interactive%20Map.png?raw=true)

**April 2015 Map**

![](https://github.com/Branth1/Project3/blob/master/April%202015.png?raw=true)

**Juan De Fuca Plate Scatter Plot**

![](https://github.com/Branth1/Project3/blob/master/Juan%20De%20Fuca%20Scatter.png?raw=true)

**Juan De Fuca Plate Map Plot**

![](https://github.com/Branth1/Project3/blob/master/Juan%20Map.png?raw=true)

## Conclusions
From the analysis conducted, the following conclusions were made:

* Looking at the bulk data we can see that there is quite a bit of activity consistently throughout the past 10 years. Looking at the map gives a sense of the plate boundaries that can be found near the pacific coast. Most of the data is seen along the plate boundaries for the Juan De Fuca Plate, Pacific Plate, Gorda Plate, and North American Plate. 

* Comparing all of these data points we find that the range of data is from a magnitude 2.5 up to maximum 7.9. The average over the ten-year period is a magnitude 3.07.

* In the map of April 2015 most of the data is seen to be along the North American Plate fault line that runs through California. The average for this time is at 3.05 and the maximum is a 6.2. The level of activity is quite high with about 100 data points recorded during this period. At this time there was one of the worst earthquakes we have seen in recent years. April 25, 2015, Nepal experienced a magnitude 7.8 earthquake that took the lives of nearly 9,000 people. The aftershocks and effects of this earthquake are visible through the seismic waves being recorded in the map shown. 

* Next, the area of highest interest is focused on the transform and divergent boundaries seen just off the coast. In this image around the Juan De Fuca Plate, the transform boundaries are seen running horizontally along the map and the divergent boundary can be seen running vertically at about -127.5 degrees. This map combined with the interactive map allows us to look for any possible trends between magnitude and boundary type. Upon closer review it begins to look like there is more activity along the transform boundaries over time and typically a larger magnitude.

* Earthquakes can be one of the most dangerous natural disasters we experience. Living in the pacific northwest we see a significant amount of seismic activity. Unlike other disasters, it is nearly impossible to warn the public before an earthquake happens. Through further research and data analysis we can attempt to better understand the movements of our earth's tectonic plates and hopefully one day be able to predict earthquakes before they happen and improve building designs to limit the economic and physical impact of large magnitude earthquakes. 


## References

Airgun Info
https://pangea.stanford.edu/~edunham/publications/Watson_etal_airguns_G19.pdf

Data Collection OOI
https://oceanobservatories.org/instrument-series/hydbba/

Earthquake Information
https://earthquake.usgs.gov/earthquakes/map/#%7B%22feed%22%3A%221583878977292%22%2C%22sort%22%3A%22newest%22%2C%22basemap%22%3A%22grayscale%22%2C%22restrictListToMap%22%3A%5B%22restrictListToMap%22%5D%2C%22timezone%22%3A%22utc%22%2C%22mapposition%22%3A%5B%5B42.3%2C-130.342%5D%2C%5B48.23%2C-124.453%5D%5D%2C%22overlays%22%3A%5B%22plates%22%5D%2C%22viewModes%22%3A%5B%22list%22%2C%22map%22%5D%2C%22listFormat%22%3A%22default%22%2C%22autoUpdate%22%3Afalse%2C%22search%22%3A%7B%22id%22%3A%221583878977292%22%2C%22name%22%3A%22Search%20Results%22%2C%22isSearch%22%3Atrue%2C%22params%22%3A%7B%22starttime%22%3A%222019-03-03%2000%3A00%3A00%22%2C%22endtime%22%3A%222019-05-05%2023%3A59%3A59%22%2C%22maxlatitude%22%3A48.23%2C%22minlatitude%22%3A42.3%2C%22maxlongitude%22%3A-124.453%2C%22minlongitude%22%3A-130.342%2C%22minmagnitude%22%3A4.5%2C%22orderby%22%3A%22time%22%7D%7D%7D

Project2c
https://github.com/Branth1/Project2
