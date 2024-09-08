---
# **Table of Contents**
---

**1.** [**Introduction**](#Section1)<br>
**2.** [**Problem Statement**](#Section2)<br>
**3.** [**Installing & Importing Libraries**](#Section3)<br>
  - **3.1** [**Installing Libraries**](#Section31)
  - **3.2** [**Upgrading Libraries**](#Section32)
  - **3.3** [**Importing Libraries**](#Section33)

**4.** [**Data Acquisition & Description**](#Section4)<br>
  - **4.1** [**Data Description**](#Section41)
  - **4.2** [**Data Information**](#Section42)

**5.** [**Data Pre-Profiling**](#Section5)<br>
  - **4.1** [**Pre-profiling report**](#Section51)
 
**6.** [**Data Cleaning**](#Section6)<br>
  - **6.1** [**Handling of Inconsistant Data**](#Section61)
  - **6.2** [**Handling of Missing Values**](#Section611)
  - **6.3** [**Dropping the necessary features**](#Section62)

**7.** [**Data Post-Profiling**](#Section7)<br>
**8.** [**Exploratory Data Analysis**](#Section8)<br>
  
- **8.1** [**How does the Day of a Week effect the number of earthhquakes?**](#Section81)
- **8.2** [**What is the relation between Day of the month and Number of earthquakes that happend in a year?**](#Section82)
- **8.3** [**What does the average frequency of earthquake in a month from the year 1965 to 2016 tell us?**](#Section83)
- **8.4** [**What is the relation between Year and Number of earthquakes that happend in that year?**](#Section84)
- **8.5** [**How is the earthquake magnitude on an average has been varied over the years?**](#Section85)
- **8.6** [**How does year impacts the standard deviation of the earthquakes?**](#Section86)
- **8.7** [**Does geographic location have anything to do with earthquakes?**](#Section87)
- **8.8** [**Where do earthquakes occur very frequently?**](#Section88)
- **8.9** [**What is the relation between Magnitude, Magnitude Type , Status and Root Mean Square of the earthquakes?**](#Section89)
<br>

**9.** [**Summarization**](#Section9)<br>

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

<center><img src = "https://raw.githubusercontent.com/insaid2018/Term-2/master/images/earthquake.PNG" ></center>

### **Scenario**

- Consider that **you are a data scientist** at NEIC.

- Your **objective** is to **perform** **EDA** on the given dataset and **come up** with **the insights**.

- Several **insights** can be **derived** utilizing different features such as magnitude, latitude, longitude, etc.

- A **deep analysis** of this data will lay the **foundation** for the **prediction** of apocalyptic **earthquakes**.
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
# **5. Data Pre-Profiling**
---
<a name = Section51></a>
### **5.1 Pre Profiling Report**

- For **quick analysis** pandas profiling is very handy.

- Generates profile reports from a pandas DataFrame.

- For each column **statistics** are presented in an interactive HTML report.

  <a name = Section9></a>

---
# **9. Summarization**
---

- **<h4>Conclusion</h4>**

    - From this case study it was analyzed that **Latitude** **Longitude**, **Depth seismic stations** and **Magnitude** are the most important features whereas, **Magnitude Error**, **Magnitude Seismic Stations**, **Horizontal Distance**, **Horizontal Error**, **Azimuthal Gap** were not that much important.
 
    - The 11th day of the month has experienced the maximum number of earthquakes whereas the 31st day has experienced the least number of earthquakes.
 
    - On the 3rd and the 8th month, it has been noticed that the number of earthquakes reported was maximum.
 
    - It was analysed that the Magnitude Type **MW** has the highest amount of magnitude whereas **MD** had the least magnitude value.


-  **<h4>Actionable Insights</h4>**

    - Manually reviewed status has performed better over automatic checks hence, manual evaluation of earthquake magnitude is advisable.   
 
    - As the oceanic region experiences a lot more seismic activity than mainland regions and most of the earthquakes have been reported to the lands connected to the **north pacific ocean**, it is advised not to perform any project or execution-based task in the 3rd and 8th month of the year in order to avoid physical consequences.

  
  
 
