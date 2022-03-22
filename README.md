# EV-operational-carbon-emission-inventory-of-US
This repository provides the data used to calculate the carbon emission of electric vehicles (EVs) in **hourly resolution** in each state of the continental United States. The calculation results will be provided soon.
## Introduction
There are three types of source data to constitute this repository.
- electricity grid operational data
- temperature data
- travel behavior data. 

All of them are publicity available.The following table describes the download address of each source data and the corresponding storage folder in this repository. All the data are in either .csv nor .xlsx format.
| Name  | Download address |Stored folder path |
| ------------- | ------------- | ------------- |
| Grid operational data | https://www.eia.gov/opendata/qb.php?category=2123635 | ./grid |
| Temperature data  | https://www.ncei.noaa.gov/metadata/geoportal/rest/metadata/item/gov.noaa.ncdc:C01626/html | ./temperature |
| Travel behavior data | https://nhts.ornl.gov/ | ./travel |

Codes are stored in the same folder of the corresponding data to facilite run the code. The code were written in Python 3 by Jupyter Notebook. So far, the code for cleaning data (i.e., build the data structure/compute the variables for next step modeling and fill in the missing data) is complete.

More detailed instructions can be found on comments of each code file.

Should you have any interest or enquiry,please contact zixuan.kang@connect.polyu.hk
