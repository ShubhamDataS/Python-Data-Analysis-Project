# Earthquake Prediction

---
### **Table of Contents**


**1.** [**Introduction**](#Section1)<br>
**2.** [**Problem Statement**](#Section2)<br>
**3.** [**Installing & Importing Libraries**](#Section3)<br>
**4.** [**Data Acquisition & Description**](#Section4)<br>
**5.** [**Data Preprocessing**](#Section5)<br>
**6.** [**Exploratory Data Analysis**](#Section8)<br>
**7.** [**Summarization**](#Section9)<br>

---
<a name = Section1></a>
# **1. Introduction**
---

- Everyone knows about **earthquakes**, and **commonly**, we all have **experienced** one.

- In **some parts** of the world, earthquakes are **common**, and in **some**, they are **rare incident**s.

- In this particular case study, we have **gathered data** on all the **earthquakes from 1965 to 2016**.

- The sole purpose of this case study is to **analyze** and **identify patterns** of an earthquake occurring.

- Apart from that, we will also **study** the **damage** caused by earthquakes and the **appropriate measures** in the future.



<a name = Section2></a>
# **2. Problem Statement**
---


- Earthquake occurs worldwide, and the information is spread immediately to global agencies, scientists, critical facilities, and the public.

- The **National Earthquake Information Center (NEIC)** determines the location and size of all significant earthquakes.

- The **NEIC** compiles and provides an extensive seismic database (as a foundation) to scientists and the public.

- The medium is the operation of **modern digital national** and **global seismograph networks** and cooperative international agreements.

<br>
---
<a name = Section3></a>
# **Installing & Importing Libraries**
---
- Installing,upgrading and importing all the libraries here such as Panada, Numpy, Plotly, Matplotlib etc.

---
<a name = Section4></a>
# **4. Data Acquisition & Description**
---

- The data is a subset of the USGS dataset and its in-depth feature information can be found <a href="https://earthquake.usgs.gov/data/comcat/index.php#horizontalError">here</a>.


</br>

| Records | Features | Dataset Size |
| :-- | :-- | :-- |
| 23412 | 21 | 2.29 MB| 

</br>

| Id | Features | Description |
| :-- | :--| :--| 
|01|**Date**|Date at which the earthquake occurred.|
|02|**Time**|Time at which the earthquake occurred.|
|03|**Latitude**|Latitude of location of earthquake.|
|04|**Longitude**|Longitude of location of earthquake.|
|05|**Type**|Type of Disasters such as Earthquake, Nuclear Explosion, Explosion and Rock Burst. |
|06|**Depth**|Depth at which earthquake occurred (in km).|
|07|**Depth Error**| An earthquake cannot physically occur at a depth of 0 km or -1km however, sometimes due to misscalculation it is reported to be negetive. |
|08|**Depth Seismic Stations**| An earthquake can occur anywhere between the Earth's surface and about 700 kilometers below the surface. |
|09|**Magnitude**|Magnitude of earthquake on Richter scale.|
|10|**Magnitude Type**| The type of Earthquake Magnitude such as MW, MWC	MB etc.|
|11|**Magnitude Error**| The difference in between true magnitude and predicted magnitude is known as  Magnitude Error. | 
|12|**Magnitude Seismic Stations**| The existence of deep-focus earthquakes was confirmed in 1931 from studies of the seismograms of several earthquakes.|
|13|**Azimuthal Gap**| The maximum angle separating two adjacent seismic stations, both measured from the epicenter of an earthquake.|
|14|**Horizontal Distance**|Horizontal distance from the epicenter to the nearest station (in degrees). 1 degree is approximately 111.2 kilometers. |
|15|**Horizontal Error**|The horizontal location error, in km. |
|16|**Root Mean Square**| The frequently used measure of the differences between values (sample or population values) predicted by a model|
|||or an estimator and the values observed is known as Seismic Attribute|
|17|**ID**|Earthquake Identifier. |
|18|**Source**|The primary network contributors of the source of event. |
|19|**Location Source**|The network that originally authored the reported location of this event. |
|20|**Magnitude Source**|The network that originally authored the reported magnitude for this event. |
|21|**Status**|Indicates whether the event has been reviewed by a human. Contains: [Automatic, Reviewed]|

<a name = Section5></a>

---
# **5. Data Profiling**
---

- For **quick analysis** pandas profiling is very handy.

- Generates profile reports from a pandas DataFrame.

- For each column **statistics** are presented in an interactive HTML report.

  <a name = Section9></a>

  <a name = Section8></a>

---
# **6. Exploratory Data Analysis**
---

---
# **7. Summarization**
---

- **<h4>Conclusion</h4>**

    - From this case study it was analyzed that **Latitude** **Longitude**, **Depth seismic stations** and **Magnitude** are the most important features whereas, **Magnitude Error**, **Magnitude Seismic Stations**, **Horizontal Distance**, **Horizontal Error**, **Azimuthal Gap** were not that much important.
 
    - The 11th day of the month has experienced the maximum number of earthquakes whereas the 31st day has experienced the least number of earthquakes.
 
    - On the 3rd and the 8th month, it has been noticed that the number of earthquakes reported was maximum.
 
    - It was analysed that the Magnitude Type **MW** has the highest amount of magnitude whereas **MD** had the least magnitude value.


-  **<h4>Actionable Insights</h4>**

    - Manually reviewed status has performed better over automatic checks hence, manual evaluation of earthquake magnitude is advisable.   
 
    - As the oceanic region experiences a lot more seismic activity than mainland regions and most of the earthquakes have been reported to the lands connected to the **north pacific ocean**, it is advised not to perform any project or execution-based task in the 3rd and 8th month of the year in order to avoid physical consequences.

  
  
 
