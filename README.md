# Risk_Map_Herring_Spawning_Areas
This risk map combines different risks for herring spawning areas to a risk value between 0 (no/ low risk) to 1 (high risk) in a hexgon grid. 

The web map is available under: https://sheilatholen.github.io/Risk_Map_Herring_Spawning_Areas/


##THE MAP
###How it was created
This map based on different raster and vector data about the risks for herring spawning areas. Therefore all datasets were clipped to the archipelago sea and a hexagongrid were created for the same area. For each hexagon, the mean of the overlapping grid cells was calculated, and the results were normalized to a scale of 1 using Min-Max normalization. Similar procedures were applied to vector layers. For the Trapnet layer (point vector), the points per hexagon were counted and normalized to 1. The Fishing Net layer is a polygon dataset, which was converted into a raster dataset. The raster cells were counted per hexagon and normalized to 1. Subsequently, the mean of all normalized values for each hexagon was calculated and normalized to 1 as well. These values represent the risk for herring spawning areas. Zero indicates no/low risk, while one represents the highest value and thus the highest risk. The hexagonal grid is colored based on the calculated risk value. This process was conducted for the years 2014 and 2018.


###How to use it
The map offers various functionalities. The hexagons represent the risk value for the herring spawning areas. The hexagons are colored based on the calculated overall risk. Clicking on an individual hexagon displays the different risk values for that hexagon as a bar plot. Hovering the mouse over a bar shows the value for the selected risk. The buttons at the top-left allow switching between the years 2014 and 2018. The button at the bottom-left enables the individual toggling of layers. The legend for the different layers is located at the bottom-right. Below this button is a coordinate display."



##Datasets

###Anthropogenic noise:
The Input of continuous anthropogenic sound HOLAS 2 –dataset has data about anthropogenic sound in the Baltic Sea. The data was collected for the BIAS (Baltic Sea Information on the Acoustic Soundscape) project. The data was collected in 2014 and the dataset created in 2018.
Available under: https://metadata.helcom.fi/geonetwork/srv/eng/catalog.search#/metadata/8e73d7ab-d683-41f5-87ad-e97445e8eee5


The Input of continuous anthropogenic sound HOLAS 3 –dataset has data about anthropogenic sound in the Baltic Sea. The data for was collected for the HELCOM BLUES (Biodiversity, Litter, Underwater noise and Effective regional measures for the Baltic Sea) project. The data was collected in 2018 and the dataset created in 2023.
Available under: https://metadata.helcom.fi/geonetwork/srv/fin/catalog.search#/metadata/d1cf5bda-fed2-4f54-a3c2-af701ed3a397)

###Shipping density:
The HELCOM (Helsinki Commission) AIS (Automatic Identification System) Shipping density maps –dataset has data about the density of all IMO (International Maritime Organization) registered ships operating in the Baltic Sea. The data was collected in years 2006-2022 and the dataset created in 2022.
Available under: https://metadata.helcom.fi/geonetwork/srv/eng/catalog.search#/metadata/2558244b-0cea-46e9-8053-af6ef5d01853

###Fishing nets & trap nets:
For fishing nets and trap nets in the Archipelago Sea we used a dataset called “Tärkeät kaupalliset kalastusalueet rannikolla: rysäpyydyspaikat ja verkkokalastusalueet”. It consists of two layers and has data about important commercial fishing areas on the Finnish coast. Data for the dataset is from Luke, ELY-keskukset and Österbottens Fiskarförbund. The data was collected in the Archipelago Sea area by interviewing fishermen during years 2010-2014 and it was published in 2020.
Available under: https://ckanmtp.ymparisto.fi/dataset/90847ce4-8879-4b04-b533-177d5a1be4fa

###Potential spawning areas for herring
The Potential spawning areas for herring (PBS EFH) -dataset has data about the potential spawning areas of herring. EFH stands for Essential fish habitat map and PBS stands for PanBalticScope project. The EFH map was created for the PBS project. This dataset was created based on scientific literature, not on actual data about herring spawning areas. That’s why it only shows potential spawning areas. The dataset was published in 2020.
Available under: https://metadata.helcom.fi/geonetwork/srv/eng/catalog.search#/metadata/bae53d8e-a5a2-4d01-b260-54d72ad46813



This map was created as part of the course Geospatial Data Management and Visualization course at the University of Turku in November 2023.
Created by: Elsa Halmajärvi, Leena Järveläinen, Sonja Rintelä, Renita Ristimäki & Sheila Tholen.
