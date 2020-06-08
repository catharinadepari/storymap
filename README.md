# storymap

<img src="img/page_front.png" width='950'> <br>
## Resilience Story of New York<br>
### :newspaper: Introduction
According to notable scholar [Holling](https://core.ac.uk/download/pdf/52941869.pdf), **`resilience`** is the persistence of relationships within a system. It is a measure of the ability of the systems to absorb changes. In the context of this storymap, the resilience is the capacity of New York State citizens to withstand a disturbance including a pandemic.<br>
The aim of this storymap is to represent the strugggles of the New York State citizens in dealing with **`the COVID-19 pandemic`** which is complicated by some economic and social facts that had long interplayed in the U.S. history.<br>
This storymap evidences the potential of digital technology in explaining a social phenomenon in a specific geographic area and to mobilze social power towards a desired change (James, Kitchin and Leszczynski 2018, 26).<br>

> *Digital Geography** is a set of technologies that go beyond an engagement with an interface, but also involve spatial big data. DUe to its social power, one even called the story map as **`human document`**[TeachMideast](https://teachmideast.org/articles/digital-geography-applications/).<br>

### :hammer: Storyline
In the web map process, I primarily developed the storyline by referring to the compeling work of [Song, Z.](https://link.springer.com/book/10.1007%2F978-3-030-04028-4). The audience of the storymap is public, in other words, it is not specified to particular groups. I used **New York State** as the locus of this story to allow me to explain the connections between different factors (social and economy) from country to city level that complicate the resilience story of New York State.<br>Among different types of **`GENRES`**  in the Roth's Taxonomy (2016), I adopted **multimedia experienced genre**  which use *layout* and *text, images, and graphics hyperlinks* to enforce **linearity**.<br>

The 3 narrative elements of this web map include:
<br>
1. **SET-UP ACT**<br>
In terms of **`settings`**, the locus of this storymap is **New York State** that comprises 62 couunties. The **`key characters`** invoved are the citizens of the **New York State** and the **Governor Andrew Cuomo**. The **problem** is the pandemic that disrupts the lives of people in the New York State and associated policy issued by Governor Cuomo that then raised public outrage and protests. The **time frame** is the current time where the pandemic and pause order are still taking place.<br>

2. **Conflict Act**<br>
The **`key issue`** of the story is the **vulnerability of people in New York State to the pandemic increases as poverty and violance firearm rates in this state are relatively higher than other states in the U.S**. To convince users, I provided thematic spatial maps (i.e., COVID-19 case, tweets over pause order, median household income, violance firearm rate, voluntary centers) in sequential and systematic/linear order. The purpose is to show the link between these themes or factors and the concentration of the issues on specific areas in New York State: Bronx and New York cities <br>.

3. **Resolution Act**<br>
The **recommendations** offered are: 1) the need of people to embrace the pandemic as a opportunity to innovate, change, and reconsider the value of social cohesion to increase resilience to pandemic; 2) working together and listening to scientists to
deal with the pandemic as suggested by local residents and shown on the last page of this web map.<br>

## :mag_right: Data Sources
This storymap used data that are compiled from various and reliable resources belong to the U.S. government, electronic mass media, organization's websites, and twitter. For creating spatial maps, most of these data, however, need to be converted into GeoJson file and  completed with additonal data such as longitude and latitude of the location of each food pantry and homeless shelter. To obtain the location coordinates, I accessed google map. The technique can be seen from the screenshot below. <br>
<img src="img/coordinates.png" width='900'><br>

For further details, I provide the storyline of this web map in the form of hand-sketch.<br>
<img src="img/coordinates.png" width='900'><br>


| Data file | Data Type | Description| Sources |
| --------- | --------- | ---------- | ------- |
| uscases.geojson | vector | Number of COVID-19 cases and tests run in the U.S. | https://github.com/datasets/covid-19/tree/master/data |
| tweets.geojson | vector | Distribution of tweets corresponding to **pause order**. Data were gathered by using tweets crawling on May 20, 2020 | Tweeter |
| nys_viol_rate.geojson | vector | Index, Violent, property and firearm rates in NY states | https://catalog.data.gov/dataset/index-violent-property-and-firearm-rates-by-county-beginning-1990/resource/d1e392ad-8377-4ca7-8b36-7c43bb275afc |
| nyspvt.geojson | vector | Median household income of New York State in 2015 with longitude and latitude coordinates | https://data.ny.gov/Energy-Environment/NYSERDA-Low-to-Moderate-Income-New-York-State-Cens/bui8-bb6g/data |
| shelter.geojson | vector | Locations of homeless shelters in Bronx in 2020 with longitude and latitude coordinates | https://www.homelessshelterdirectory.org/cgi-bin/id/city.cgi?city=bronx&state=NY |
| food.geojson | vector | location of food pantries in Bronx and surrounding in May 2020 with longitude and latitude coordinates | https://www.foodpantries.org/ci/ny-bronx |

## :books: Libraries
Below is the table that shows the data library of two geometric/spatial files used in this leaflet: **`airports.geojson`** and **`us-states.geojson`**.

| **Library**       | **Version** | **Function**                                                                                                                   |
| ----------------- | ----------- | ------------------------------------------------------------------------------------------------------------------------------ |
| leaflet.css       | 1.4.0       | Codes for storymap making (e.g., events, animation)                                                                            |
| ajax              | 3.5.2       | Animation                                                                                                                      |
| googleapis        |             | Fonts and stylesheets                                                                                                          |
| fontawesome       | 5.7.2       | Icon markers                                                                                                                   |
| chroma            | 1.3.4       | Colors setting (e.g., chloropleth)                                                                                             |
| jquery            | 3.2.1       | Animation                                                                                                                      |
| popper.js         | 1.14.0      | Positioning engine by calculating the position of an element to make it possible to position it near a given reference element |
| bootstrap.min.css | 4.3.1       | Building responsive web map through complied source codes of css and js                                                        |
| leaflet-ajax      | 2.1.0       | Asynchronously adding geojson data                                                                                             |
| topojson.min.js   |             | Etension of GeoJSON that encodes topology                                                                                      |
| storymap          | 2.5         | Support storymap and make it robust and lightweight                                                                            |

The basemap used for this storymap is attributed to cartodb_basemaps with code as follows:
```
cartodb_dark: {
  layer: L.tileLayer('http://cartodb-basemaps-{s}.global.ssl.fastly.net/dark_all/{z}/{x}/{y}@2x.png', {
    attribution: "Generated by QMetaTiles",
    detectRetina: true
```
The miniglobe added to the storymap was retrieved from Chris Whong's leaflet example in the github with URL: https://github.com/chriswhong/leaflet-globeminimap/blob/master/example/index.html.

## :flags: Credits/Acknowledgement
The credits are directed to:
- New York State Government for its open source database that allows the storymap to be developed
- New York State's food pantry and homeless shelters database
- U.S. Center of Disease Control and Prevention for providing recent data of COVID-19 cases in the U.S.
-  for the inspiring video of New York's streets during the pandemic
- Social media: *New York Times*, *Los Angeles Times*, for providing the current information that relate with the pandemic in New York State
-
- Professor Bo Zhao for advisory and guidance that allows the improvement for this storymap possible to be made
- students of GEOG 458 in University of Washington for the peer-reviewing <br>

### :link: References <br>
[1] Holling:  <https://core.ac.uk/download/pdf/52941869.pdf> <br>
[2] TeachMideast](https://teachmideast.org/articles/digital-geography-applications/ <br>
[3] [Song, Z.](https://link.springer.com/book/10.1007%2F978-3-030-04028-4) <br>
[4] Laflet Plugin <https://leafletjs.com/plugins.html> <br>
