# Project4
Shared Colab Link:
https://colab.research.google.com/github/Branth1/Project4/blob/master/Project4b.ipynb

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

First is an attempt to capture Air gun frequency on the Axial Base Seafloor. Second is an attempt to capture Marine Mammal Vocalizations in the Oregon Slope Base Seafloor and finally an earthquake recorded by the Oregon Shelf Cabled Benthic Experiment Package.

## Background

**The questions we are looking to solve are as follows:**

        1-What is the effect of wind and rain on underwater noise?

        2-Which one has the highest impact? Rain or Wind?

        3-What are the main reasons for observing different spectral levels in Oregon shelf compared to Oregon offshore?

        4-Compare the three bandwidths of the signals recorded in the Spectrograms. 

        5-Are they consistent with what is shown in the Wenz curve?

**The Data used for analysis is:**

To view the individual data sets please follow the link above to the colab code. All data links are located in their corresponding sections.

Note: To determine the time periods of wind and or rain, Project2 was used. The link to this project is found under references below. For each of the 4 different weather requirements, a minimum or 3 consistent hours was first identified. Then a 5-minute window near the middle of the data set was selected for hydrophone data analysis. There may be some discrepancies due to the method of selecting these time windows. Since the previous project had hour time intervals, it is possible that the weather conditions needed are not present at the time of analysis.

Additionally, the earthquake data used to determine the time window was found from the USGS website. The link is located in references below.

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

**Air gun Spectrogram**

![](https://github.com/Branth1/Project4/blob/master/Airgun.png?raw=true)

**Marine Mammal Vocalization Spectrogram**

![](https://github.com/Branth1/Project4/blob/master/Marine%20Mammals.png?raw=true)

**Earthquake Spectrogram**

![](https://github.com/Branth1/Project4/blob/master/EQF.png?raw=true)

## Conclusions
From the analysis conducted, the following conclusions were made:

* When looking at the graphs of weather patterns, it can be seen that the wind and rain raise the PSD throughout the frequency range. The wind appears to create more drastic spikes in energy than rain. However, the rain still causing an overall energy increase when compared to no wind and no rain. 

* It seems that wind has the highest impact instantaneous impact on the energy at each location. However, when looking at the Oregon Shelf we can see that through the entire frequency range, the rain raises the mean above both the no wind no rain case and the wind no rain case. Although, this is not as prominent in the Oregon Offshore situation. 

* One of the main reasons we see different SPD levels between the two sites would have to do with location. It is important to note that the Oregon Shelf site has a depth of 80m while the Oregon Offshore site has a depth of 580m. Although, there may be some inaccuracies in the data as previously discussed, we can clearly see that the Oregon Shelf site ranges for PSD are higher in all cases.

* When comparing the spectrogram's, the air gun was rather tricky to locate. However, it appears to be visible in the image above with a Bandwidth of about 25-75 Hz. The marine mammal vocalization appears a bit higher with a bandwidth of just under 500 and up to about 3500 Hz. The earthquake was attempted to be captured at the time of initiation. According to USGS, a magnitude 4.7 earthquake hit off the Oregon Coast on 4/10/19 at 14:11:31. Notice, the earthquake is visible in the end of the recording. A longer data file was used to improve the clarity of changes. However, since it was such a large amount of data, the detail was reduced to increase speed of processing. In it we can see the increasing bandwidth with the range of 0-100 Hz and a little more. The graphs shown have had the ranges adjusted to improve clarity. 

* When comparing these values to the Wenz curve shown above, they seem to fit the expected curve and applicable ranges. We can see that earthquakes are expected between 0-100 Hz, marine mammal vocalization is in the higher ranges up into the multiple kHz, and air guns are expected to fit the explosion range of 0-100 Hz to try and reduce impact on marine mammal environment. Although they have higher frequencies which must be addressed, that is beyond the scope of this analysis. Additional information on this topic can be found in references. In addition, we can see that this curve appears to hold true for the weather patterns as well. Wind having the higher frequency and greater spectral density than rain, where rain depends on the sea state.

For further information on OOI, the work that they do and to view additional datasets for analysis, please visit the links below. 


## References

Air gun Info
https://pangea.stanford.edu/~edunham/publications/Watson_etal_airguns_G19.pdf

Data Collection OOI
https://oceanobservatories.org/instrument-series/hydbba/

Earthquake Information
https://earthquake.usgs.gov/earthquakes/map/#%7B%22feed%22%3A%221583878977292%22%2C%22sort%22%3A%22newest%22%2C%22basemap%22%3A%22grayscale%22%2C%22restrictListToMap%22%3A%5B%22restrictListToMap%22%5D%2C%22timezone%22%3A%22utc%22%2C%22mapposition%22%3A%5B%5B42.3%2C-130.342%5D%2C%5B48.23%2C-124.453%5D%5D%2C%22overlays%22%3A%5B%22plates%22%5D%2C%22viewModes%22%3A%5B%22list%22%2C%22map%22%5D%2C%22listFormat%22%3A%22default%22%2C%22autoUpdate%22%3Afalse%2C%22search%22%3A%7B%22id%22%3A%221583878977292%22%2C%22name%22%3A%22Search%20Results%22%2C%22isSearch%22%3Atrue%2C%22params%22%3A%7B%22starttime%22%3A%222019-03-03%2000%3A00%3A00%22%2C%22endtime%22%3A%222019-05-05%2023%3A59%3A59%22%2C%22maxlatitude%22%3A48.23%2C%22minlatitude%22%3A42.3%2C%22maxlongitude%22%3A-124.453%2C%22minlongitude%22%3A-130.342%2C%22minmagnitude%22%3A4.5%2C%22orderby%22%3A%22time%22%7D%7D%7D

Project2c
https://github.com/Branth1/Project2

Wenz Curve
https://dosits.org/science/sounds-in-the-sea/what-are-common-underwater-sounds/
