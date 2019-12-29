## Integration of Roadside Camera Images and Weather Data for Monitoring Winter Road Surface Conditions

This repository contains the data and source code of the [CARSP'19](http://www.carsp.ca/past-conferences/carsp-conference-2019/) paper titled *Integration of Roadside Camera Images and Weather Data for Monitoring Winter Road Surface Conditions*, it also uncludes PDF documents of the paper and the slides.

This was awarded as the **best paper in the student competition**. The official proceedings are available in [CARSP](http://www.carsp.ca/research/research-papers/proceedings/2019-calgary/).

Authors: *Juan Carrillo <sup>1</sup>, Mark Crowley <sup>1</sup>.*

* *<sup>1</sup> University of Waterloo. Canada*

### Abstract
> During the winter season, real-time monitoring of road surface conditions is critical for the safety
of drivers and road maintenance operations. Previous research has evaluated the potential of
image classification methods for detecting road snow coverage by processing images from
roadside cameras installed in RWIS (Road Weather Information System) stations. However, there
are a limited number of RWIS stations across Ontario, Canada; therefore, the network has
reduced spatial coverage. In this study, we suggest improving performance on this task through
the integration of images and weather data collected from the RWIS stations with images from
other MTO (Ministry of Transportation of Ontario) roadside cameras and weather data from
Environment Canada stations. We use spatial statistics to quantify the benefits of integrating the
three datasets across Southern Ontario, showing evidence of a six-fold increase in the number of
available roadside cameras and therefore improving the spatial coverage in the most populous
ecoregions in Ontario. Additionally, we evaluate three spatial interpolation methods for inferring
weather variables in locations without weather measurement instruments and identify the one that
offers the best tradeoff between accuracy and ease of implementation.

### Keywords
Data integration, Spatial Statistics, Road Monitoring, Weather sensors, Roadside cameras.

### Remark
By adding all other MTO cameras as image data sources to the RWIS system, **six times more cameras are available**. Adding weather stations from Environment Canada to the RWIS system increases the number of weather stations by 1.7x.

### Input data
For this project we use multiple datasets listed below. All are published here in Shapefile format and projected in the [EPSG:3347](https://epsg.io/3347) coordinate reference system. Figure 1 shows a graphical overview of the datasets.

<img src="/readme-images/datasets_map.png" width="450" />

*Figure 1. Location of data collection stations from the three input systems.*

#### Data retrieved from StatCan
* **[ontario_boundary](/data/ontario_boundary.zip)**: Official boundary of the Province of Ontario. 
* **[ontario_three_populous_ecoregions](/data/ontario_three_populous_ecoregions.zip)**: Official boundaries of the three most densely inhabited ecoregions in Ontario. 

#### Data provided by the [iTSS LAB](https://itsslab.com/) at the University of Waterloo
* **[ontario_all_rwis_stations](/data/ontario_all_rwis_stations.zip)**: Locations of all 139 Road Weather Information System (RWIS) stations.
* **[rwis_40_sample_stations](/data/rwis_40_sample_stations.zip)**: Locations and weather data for a sample of 40 Road Weather Information System (RWIS) stations.

#### Data retrieved from Environment Canada
* **[ontario_all_envcan_stations](/data/ontario_all_envcan_stations.zip)**: Locations of all 99 Environment Canada weather stations in Ontario.
* **[envcan_40_sample_stations](/data/envcan_40_sample_stations.zip)**: Locations and weather data for a sample of 40 Environment Canada weather stations in Ontario.

#### Data retrieved from the Ministry of Transportation of Ontario (MTO)
* **[ontario_all_mto_stations](/data/ontario_all_mto_stations.zip)**: Locations of all 439 MTO roadside cameras in Ontario.

### Acknowledgements

<img src="/readme-images/conference_image.png" width="550" />

Juan Carrillo was supported for this project by the University of Waterloo [Machine Learning Lab](https://uwaterloo.ca/scholar/mcrowley/lab). Special thanks to Professor Mark Crowley for his mentoring and contributions during this research project. Last but not least thanks to the Canadian Association of Road Safety Professionals CARSP for organizing the Conference.
