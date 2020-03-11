# Project4
Shared Colab Link:
https://colab.research.google.com/github/Branth1/Project3/blob/master/Project3.ipynb

GitHub Link:
https://github.com/Branth1/Project4
## Description

This is a study of some Hydrophone data collected by the Ocean Observatory Initiative (OOI). 

The OOI is a major research equipment and facilities construction project funded by the National Science Foundation. It consists of seven arrays of sensors located across the North and South Atlantic and Pacific, including one cabled, two coastal, and four global arrays.

The data sets being studied and compared below will focus on Hydrophone data collected from:

Oregon Shelf Cabled Benthic Experiment Package

Oregon Offshore Cabled Benthic Experiment Package

Axial Base Seafloor

Oregon Slope Base Seafloor

For the first section we will look at the Oregon Shelf and Oregon Offshore in which we will compare the Power Spectral Density to frequency in four different weather conditions.

        1-No Wind and No Rain

        2-Wind and No Rain

        3-Rain and No Wind
        
        4-Wind and Rain

After this, a Spectrogram is created for 3 additional data sets.

First is an attempt to capture Airgun frequency on the Axial Base Seafloor. Second is an attempt to capture Marine Mammal Vocalizations in the Oregon Slope Base Seafloor and finally an earthquake recorded by the Oregon Shelf Cabled Benthic Experiment Package.

## Background

**The questions we are looking to solve are as follows:**

        1-What is the effect of wind and rain on underwater noise?

        2-Which one has the highest impact? Rain or Wind?

        3-What are the main reasons for observing different spectral levels in Oregon shelf compared to Oregon offshore?

        4-Compare the three bandwidths of the signals recorded in the Spectrograms. 

        5-Are they consistent with what is shown in the Wenz curve?

**The Data used for analysis is:**

To view the individual data sets please follow the link above to the colab code. All data links are located in their corresponding sections.

Note: To determine the time periods of wind and or rain, Project2 was used. The link to this project is found under references below. For each of the 4 different weather requirements, a minimum or 3 consistent hours was first identified. Then a 5 minute window near the middle of the data set was selected for hydrophone data analysis. There may be some discrepencies due to the method of selecting these time windows. Since the previous project had hour time intervals, it is possible that the weather conditions needed are not present at the time of analysis.

Additionaly, the earthquake data used to determine the time window was found from the USGS website. The link is located in references below.

For additional information on the analysis used please see the link to the code above.

## Solution/Results

The data was analyzed utilizing the code found in the link above. First the Fourier Transform is taken for 1 second intervals of the raw hydrophone data from each sample set. This is used to calculate the power spectral density using the following equation:

![](https://github.com/Branth1/Project4/blob/master/PSD.png?raw=true)

This is then converted to dB and plotted against frequency for each site with the 4 different weather patterns.

For the second portion the Spectrograms are created, analyzed and compared with the Wenz curve shown below:

![](https://github.com/Branth1/Project4/blob/master/Wenz%20curve.png?raw=true)


**Initial Data Analysis**

Note: For the following graphs, the specific days and time being analyzed can be found and additional data sets can be tested utilizing the code found above and the OOI website.

**Oregon Shelf Cabled Benthic Experiment Package**

![](https://github.com/Branth1/Project4/blob/master/Oregon%20Shelf.png?raw=true)

**Oregon Offshore Cabled Benthic Experiment Package**

![](https://github.com/Branth1/Project4/blob/master/Oregon%20Offshore.png?raw=true)

**Airgun Spectrogram**

![](https://github.com/Branth1/Project4/blob/master/Airgun.png?raw=true)

**Marine Mammal Vocalization Spectrogram**

![](https://github.com/Branth1/Project4/blob/master/Marine%20Mammals.png?raw=true)

**Earthquake Spectrogram**

![](https://github.com/Branth1/Project4/blob/master/Earthquake.png?raw=true)

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

Wenz Curve
https://dosits.org/science/sounds-in-the-sea/what-are-common-underwater-sounds/
