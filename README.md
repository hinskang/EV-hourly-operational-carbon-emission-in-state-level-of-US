# EV-operational-carbon-emission-inventory-of-US
This repository provides the data used to calculate the carbon emission of electric vehicles (EVs) in **hourly resolution** in each state of the continental United States. The calculation results will be provided soon.
## Introduction
There are three types of source data to constitute this repository.
- electricity grid operational data
- temperature data
- travel behavior data. 

All of them are publicity available.The following table describes the download address of each source data and the corresponding storage folder in this repository. All the data are in either .csv or .xlsx format.
| Name  | Download address |Stored folder path |
| ------------- | ------------- | ------------- |
| Grid operational data | https://www.eia.gov/opendata/qb.php?category=2123635 | ./grid |
| Temperature data  | https://www.ncei.noaa.gov/metadata/geoportal/rest/metadata/item/gov.noaa.ncdc:C01626/html | ./Temperature |
| Travel behavior data | https://nhts.ornl.gov/ | ./Travel |

Codes are stored in the same folder of the corresponding data to facilite running the code. The code were written in Python 3 by Jupyter Notebook. So far, the code for cleaning data (i.e., build the data structure/compute the variables for next step modeling and fill in the missing data) is complete.

More detailed instructions can be found on following sections and comments of each code file.

Should you have any interest or enquiry,please contact zixuan.kang@connect.polyu.hk

## Instruction for grid folder
This folder contains the following three types of open-access data provided by U.S. Energy Information Administration (EIA). The data covers the whole continental United States. All of the data are in hourly resolution. The following table shows the name of data and the corresponding storage loaction in this repository.

| Name  | Stored folder path |
| ------------- | ------------- |
| regional electricity consumption data | ./grid/elec_consumption.rar |
| regional electricity generation data  | Pending to upload |
| region-to-region electricity interchange data | ./grid/elec_Interchange.rar |

The data of each region are stored in a sperate .xlsx file. The so-called regions refers to the houly electric grid region defined by U.S. EIA. A visual look can be seenn at https://www.eia.gov/electricity/gridmonitor/dashboard/electric_overview/US48/US48. 

The code in this folder is reponsible for filling in the missing data for each .xlsx file and aggregating them into a single .xlsx file in a specific data structure to facilitate the later modeling analysis. Computational results are pending to upload.

## Instruction for temperature folder
This folder contains a 15-year temperature data from 2006-2020 across the whole continental United States. They are the latest temperature bulk data provided by U.S. national oceanic and atmospherric administration (NOAA), while most previous academic studies used the data from 1981-2010.

The source data is in station-level. The code in this folder is reponsible for excluding the missing data and aggregating the station-level data into a state-level.

The source data is pending to upload.

## Instruction for travel folder
This folder contains the 2017 national household travel survey data provided by U.S.department of transportation, federal highway administration. The code for this folder is still pending to finish.
