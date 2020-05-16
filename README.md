# storymap

<img src="img/leaflet_airport.png" width='950'> <br>
## Resilience Story of New York in the Face of COVID-19<br>
### :newspaper: Introduction
The aim of this project is to visualize the spatial distribution of airport's traffic control tower in the U.S. Air traffic control tower or **`ATCTs`** .<br>

<1> 'I <symbol love>Love New York' & Hate Coronavirus
<1a> New York Before COVID-19
<1b> Cases and Spread of COVID-19
<2> The Dilema
<2a> Lockdown, Self-Quarantine, & Social Distancing
<2b> From Protests, Gunfires, to Reopenings
<3> The Beauty 'of' the Beast
<3a> Social Cohesion
<3b> Heroism
<3c> Innovation
<4> Resilience & Change the Mindset

Reopening:
<iframe width="476" height="267" src="" frameborder="0" allowfullscreen></iframe>

### :hammer: Storyline
The primary functions used to create the spatial map are :
- **`var mymap = L.map()`** for initializing the map and set its view related to geographical coordinates and a zoom level.
-<br>

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

## :mag_right: Data Resources
The two data files are obtained from two different sources as described below:
| Name of data file   | Data Format      | Description | Source |
| ------------------- | ----------------------- | ----------- | ------ |
| *airports.geojson*  | geojson/ geometric data | contains all the airports in the United States |<https://catalog.data.gov/dataset/usgs-small-scale-dataset-airports-of-the-united-states-201207-shapefile>|
| *us-states.geojson* | geojson/ geometric data | containing all the states' boundaries of the United States |https://bost.ocks.org/mike/|
| basemap | tile layer | a tile layer for the basemap | <http://leaflet-extras.github.io/leaflet-providers/preview/> |

## :bulb: Analysis
There are two interpretations that can be drawn from this spatial map where red icon represents the availability of ATCTs and yellow icon indicates the unavailability of ATCTs.
- ***First***, the  <br>

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

# The Guideline for Essay

You are expected to write a essay to analyze a digital-geography-related project (e.g., web map, smart dashboard, geo-narrative, etc.). You are aiming for **no less than 1500 words** coalescing around the examined digital-geography project and readings from this quarter.

 Through writing this essay, you are expected to use the learned knowledge and skill set to holistically examine the project's functions and critically reflect upon its social implications. This essay can be simple and focus in nature, but must include the following features:

- create a dedicated github repository, and write this essay on a readme.md file of this repo.
- introduce this digital-geography project, including, but not limitedt to,
  - the goal of this project (why this project was made?)
  - the major functions
  - the targeting audience
  - the authors and their affilication
- describe the systematic architecture
  - client, server, services, and data.
- inspect the code of this project, especially look into the following issues.
  - What are the data flowed in between the client and server.
  - The major libaries in use and their functions.
  - Does this project support responsive design?
- list the data sources
  - vectors (i.e., geojson)
  - rasters (i.e., tilelayer)
  - critique its overalll UI/UX and Web Mapping design if it has.
- describe the basemap, the thematic layer and the interactive features if it has.
- list any web map element in use (e.g, scalar bar, north arrow, legend, etc.) if it has.
- analyze the strengths and weakness of the examined project.
- disucss anything else you feel worthy to share.
- reflect upon this project with some social theories, such as digital divide, power relationship, surveillance and/or resistance.

Since the essay is written in mardown syntax, please try your best to include the following four structure or contents:

- list, highlight,
- images such as screenshot.
- code snippet
- table

##Submission

Please submit the url link of your essay to the final project submission tab on Canvas. Essay is due no later than the end of **Week 10**.


>  **Note:** The requirements to the essay may be slightly changed according the progress of this course. The final requirements are subject to the instructor's notification.
