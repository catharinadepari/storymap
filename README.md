# storymap

<img src="img/page_front.png" width='950'> <br>
## Resilience Story of New York<br>
### :newspaper: Introduction
According to notable scholar [Holling](https://core.ac.uk/download/pdf/52941869.pdf)]), **`resilience`** is the persistence of relationships within a system. It is a measure of the ability of the systems to absorb changes. In the context of this storymap, the resilience is the capacity of New York State citizens to withstand a disturbance including a pandemic.<br>
The aim of this storymap is to represent the strugggles of the New York State citizens in dealing with **`the COVID-19 pandemic`** which is complicated by some economic and social facts that had long interplayed in the U.S. history.<br>
This storymap evidences the potential of digital technology in explaining a social phenomenon in a specific geographic area and to mobilze social power towards a desired change (James, Kitchin and Leszczynski 2018, 26).<br>

> *Digital Geography** is a set of technologies that go beyond an engagement with an interface, but also involve spatial big data. DUe to its social power, one even called the story map as **`human document`**[TeachMideast](https://teachmideast.org/articles/digital-geography-applications/).<br>

### :hammer: Storyline
In the web map process, I primarily developed the storyline by referring to the compeling work of [Song, Z.](https://link.springer.com/book/10.1007%2F978-3-030-04028-4). The audience of the storymap is public, in other words, it is not specified to particular groups. I used **New York State** as the locus of this story to allow me to explain the connections between different factors (social and economy) from country to city level that complicate the resilience story of New York State.<br>Among different types of **`GENRES`**  in the Roth's Taxonomy (2016), I adopted **multimedia experienced genre**  which use *layout* and *text, images, and graphics hyperlinks* to enforce **linearity**.<br>

The 3 narrative elements of this web map include:
<br>
1. **SET-UP ACT**<br>
In terms of **`settings`**, the locus of this storymap is **New York State** that comprises 62 couunties. The **`key characters`** invoved are the citizens of the **New York State** and the **Governor Andrew Cuomo**. The **problem** is the pandemic that disrupts the lives of people in the New York State and associated policy issued by Governor Cuomo that then raised public outrage and protests. The **time frame** is the current time where the pandemic and pause order are still taking place.<br>
<img src="img/NY_governor.jpg" width='600'><br>

2. **Conflict Act**<br>
The **`key issue`** of the story is the **vulnerability of people in New York State to the pandemic increases as poverty and violance firearm rates in this state are relatively higher than other states in the U.S**. To convince users, I provided thematic spatial maps (i.e., covid-19 case, tweets over pause order, median household income, violance firearm rate, voluntary centers) in sequential and systematic/linear order. The purpose is to show the link between these themes or factors and the concentration of the issues on specific areas in New York State: Bronx and New York cities <br>.
<img src="img/NY_governor.jpg" width='600'><br>

3. **Resolution Act**<br>
The **recommendations** offered is the need of people to embrace the pandemic asa opportunity to innovate, change, and value solidarity as the most important asset to withstand the pandemic. improve their quality are assessing the land's suitability for oil and gas leasing through comprehensive planning processes, engaging community in the planning, raising the national minimum bid from $2.00 per acre to at least $10.00 per acre, and setting up a reliable evaluation to evaluate the lessees' capacity of exploring and producing oil and gas <br>

The primary functions used to create the spatial map are :
- **`var mymap = L.map()`** for initializing the map and set its view related to geographical coordinates and a zoom level.
-<br>

## :mag_right: Data Sources
The two data files are obtained from two different sources as described below:
| Name of data file   | Data Format      | Description | Source |
| ------------------- | ----------------------- | ----------- | ------ |
| *airports.geojson*  | geojson/ geometric data | contains all the airports in the United States |<https://catalog.data.gov/dataset/usgs-small-scale-dataset-airports-of-the-united-states-201207-shapefile>|
| *us-states.geojson* | geojson/ geometric data | containing all the states' boundaries of the United States |https://bost.ocks.org/mike/|
| basemap | tile layer | a tile layer for the basemap | <http://leaflet-extras.github.io/leaflet-providers/preview/> |

## :books: Libraries
Below is the table that shows the data library of two geometric/spatial files used in this leaflet: **`airports.geojson`** and **`us-states.geojson`**.

| **data file**      | **attribute** | **type of data** | **description** |
| ------------------ | ------------- | --------- | --------------- |
| airports.geojson   | AIRPRTX010    | Numeric    | airport tax |
| | ICAO | String | four-letter alphanumeric code designating each airport around the world, determined by International Civil Avian Organization.|
| | IATA | String | International Air Transport Association, the official trade organization for the world's airlines|
| | AIRPT_NAME | String | name of the airport in the U.S.|
| | CITY | String | the city within which the airport is located|
| | STATE | String | the state within which the airport is located |
| | COUNTY | String | the county within which the airport is located|
| | TOT_ENP | Numeric | the total number of passengers enplanned by one aircraft |
| | ELEV | Numeric | the elevation level of the airport above the sea level |
| | CNTL_TWR | Binary | the avaiilability of ATCTs where *Y* indicates availability and *N* indicates the otherwise |
| us-states.geojson | id | Numeric| identification number of the airport according to FAA. |                         |
| | name | String | name of the State where the airport is located |
| | count | Numeric | number of airports had by the state |

There are 52 features contained in the **`us-state.geojson`** file and 940 features contained in the **`airports.geojson`** file.


## :flags: Credits/Acknowledgement
The credits for this project go to:
- Professor Bo Zhao, the instructor of the GEOG 458 A at the University of Washington for the teaching materials and knowledge sharing.
- United States Government for providing the data file through its open-sourced database.
- Mike Bostock whose website is inspirational for  further leaflet exercises and provides data file for this project.
- Carto DB for providing the basemap.
- Patiphan Phengpao whose stategy of developing live server for leaflet preview (besides Atom and Google Chrome) is highly contributive <https://www.youtube.com/watch?v=FHOcQdu1iFM>. <br>

### :link: References <br>
[1] Aviation consultant DWU:  <https://dwuconsulting.com/> <br>

[4] Laflet Plugin <https://leafletjs.com/plugins.html>

In this lab, you are asked to make a storymap using the library `storymap.js`. This storymap.js library is hosted at [https://github.com/jakobzhao/storymap](https://github.com/jakobzhao/storymap). Your storymap will at least have the following features:

- In the readme file, please describe the storyline of your story map. You may refer to the lecture notes on three-action (step, confrantation, and resolution). (**10 POINTS**)

- At least 5 scenes. The content of the scenes can be obtained from Internet, historical archives, or even writing up by yourself. If you would like to use an external sources, please do mention their contribution in your credits information; (**10 POINTS**)

- At least two types of layers (e.g., tileLayer or geojson layer). These layers can be made by yourself or from other web map providers; (**10 POINTS**)


- The storymap should at least include the following controls.

    - A favicon; (**5 POINTS**)

    - customized fonts for the texts of the storymap; (**5 POINTS**)

    - A video or image on the front or end page; (**5 POINTS**)

    - A social media button to share the storymap to Facebook or Twitter; (**5 POINTS**)

    - credit information or acknowledgement;

    - A github button to point to your github repository.

The structure of your github repository should like something below.

```Powershell
[Submission_Lab_05]
│   readme.md
│   index.html
├─assets
├─js
├─css
├─img
```

## Deliverable

Once you complete this lab assignment, please make sure both the github repository and the web site work appropriately. Then, you will need to submit the url of the GitHub repository to **Canvas Dropbox**. (On the assignment tab,  press the `Submit Assignment` button to submit. Please contact the instructor or TA if you have any difficulty.)
