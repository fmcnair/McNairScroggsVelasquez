# McNairScroggsVelasquez

## Summary

The purpose of this repository is to contain all project files and data that was used for our study. The repository allows for the sharing of data and information between members of the research group. 
Our research is on Cape Fear River basin's water monitoring stations. The data we use is from four stations: East Cribbing, Loosin Creek, Research Creek, and Zeke's Basin. 
The goal of our analysis is to study the potential for eutrophication in the basin. We look at the nutrients in the water and the water quality and compare them over a 12 year period, from 2002-2024. We conduct analyses on dissolved oxygen and chlorophyll given that they can deeply impact the health of the aquatic ecosystem. We also conduct a time series analyses for each monitoring station of dissolved oxygen and chlororphyll.

## Investigators

Flannery McNair, Andi Scroggs, and Alonso Velasquez 

## Keywords

Water quality, eutroohication, dissolved oxygen, chlorophyll, time series, nutrients, and phytoplankton.

## Database Information

The data used in this research was collected by the National Estuarine Research Reserve (NERR) System's National Monitoring Program. NERR is in paid partnership with the National Oceanic and Atmospheric Administration (NOAA). We collected the data from NERR's Centralized Data Management Office on December 3, 2025. 

## Folder structure, file formats, and naming conventions 

The three folders in the repository include Code, Data, and Output. The code file includes our README.md document and our Rmd file including the code of our study. The data file includes files of our raw data and our processed data. The raw data file has all of the individual files we downloaded from the NERR Centralized Data Management Office, all of which are .csv files. The processed data is the data that we wrangled and used in our study. The output folder contains the pdf final product of our research.
The names of our files are clear and say what they contain in their names. The Rmd file is the last names of the researchers in our group. The raw data is named after the station ID's given by NERR. The "-nut" stands for nutrient and the folders with this at the end of the station ID's contain the nutrient data. The "-wq" stands for water quality. The folders with this at the end of the station ID's contain the water quality data from that station.

- NOCEC - East Cribbing
- NOCLC - Loosin Creek
- NOCRC - Research Creek
- NOCZB - Zeke's Basin

## Metadata

Raw Data

Water quality data files contain these columns of data:
- a date/time stamp (local standard time)
- a historical and provisional plus column indicating the status of QAQC
- a parameter value column; consult the metadata for the list of station and parameter codes
- a parameter flag column (the parameter header is preceded by a F_); refer to the QA Flags section below for the flag codes and descriptions
- a parameter error code column (the parameter header is preceded by EC_) MAY be present in the file depending on export type; refer to the QA Flags section below.
  
Water quality parameters:
- Temp: water temperature measured in degrees Celsius (C)
- SpCond: specific conductivity measured in milli-Siemens per centimeter (mS/cm)
- Sal: salinity measured in parts per thousand (ppt)
- DO_pct: dissolved oxygen measured in percent saturation (%)
- DO_mgl: dissolved oxygen concentration measured in milligrams per Liter (mg/L)
- Depth: sonde depth measured in meters (m)
- cDepth: depth from a non-vented sensor corrected for changes in barometric pressure (m)
- Level: sonde depth as referenced to a known vertical datum, NAVD88, measured in meters (m). 
- cLevel: level from a non-vented sensor corrected for changes in barometric pressure (m).
- pH: pH measured in standard units
- Turb: turbidity measured in nephelometric turbidity units (NTU)
- ChlFluor: chlorophyll fluorescence measured in micrograms per Liter (ug/L)*
*ChlFluor is an optional SWMP supported parameter*

Nutrient data file contains the following columns of data: 
- a date/time stamp column (local standard time)
- a historical and provisional plus column indicating the status of QAQC
- a collection method column where a 1 indicates it's a monthly grab sample and a 2 indicates it's a monthly diel sample
- a rep column indicating the sample replicate number (1, 2, 3 or S if a diel and grab sample occur at the same station, date and time)
- a parameter value column (consult the metadata for the list of station and parameter codes)
- a parameter flag column (the parameter header is preceded by a F_); refer to the QA Flags section below for the flag codes and descriptions 
- a parameter error code column (the parameter header is preceded by EC_) MAY be present in the file depending on export type; refer to the QA Flags section below.
- a comment code column in (yearly files prior to 2007 only; the parameter header is followed by a _C); refer to the QA Flags section below for the flag codes and descriptions

Nutrient parameters:
- PO4F: orthophosphate measured in milligrams per Liter (mg/L)
- NH4F: ammonium measured in milligrams per Liter (mg/L)
- NO2F: nitrite measured in milligrams per Liter (mg/L)
- NO3F: nitrate measured in milligrams per Liter (mg/L)
- NO23F: nitrite + nitrate measured in milligrams per Liter (mg/L)
- CHLA_N: chlorophyll a measured in micrograms per Liter (ug/L)

QA/QC:
All NERR SWMP data incur primary data QAQC at the CDMO within one week of data retrieval as the provisional data are ingested into the CDMO database. The data are then emailed back to the Reserve where Reserve staff use tools provided by the CDMO, Microsoft Excel macros, to perform secondary QAQC on the data. Data that have been through secondary QAQC are submitted back to the CDMO quarterly and again annually; these data are posted as provisional plus.  After annual submission to the CDMO is complete, the data undergo final tertiary QAQC by the CDMO.  The data and its accompanying metadata documentation are checked for completeness before dissemination as authenticated historical data via the CDMO Online Data Information Server (http://cdmo.baruch.sc.edu).

Processed Data

Water quality data: 
- Year in which the sample was collected
- Month in which the sample was collected
- Station Code where the sample was taken from (NOCEC, NOCLC, NOCRC, NOCZB)
- Temperature of the water measured in degrees Celsius (C)
- Salinity measured in parts per thousand (ppt)
- DO_Pct - dissolved oxygen measured in percent saturation (%)
- DO_mgl - dissolved oxygen concentration measured in milligrams per Liter (mg/L)
- Depth measured in meters (m)
- pH measured in standard units
- Turbidity measured in nephelometric turbidity units (NTU)
- NERR Site ID - ID given by NERR to identify the state where the sample was taken (NOC)
- Station Name -  Full name of the station in which the sample was taken
- LatLong - coordinates in degrees of where the sample was taken
- Latitutde in radians
- Longitude in radians
- Status of the monitoring station site the sample was from ("active" or "inactive")
- State in the U.S. where the sample was taken ("NC")
- Reserve Name - state of the U.S where the sample was taken ("North Carolina")
- Date in which the sample was collected

Nutrient data:
- Year in which the sample was collected
- Month in which the sample was collected
- StationCode where the sample was taken from (NOCEC, NOCLC, NOCRC, NOCZB)
- PO4F - orthophosphate measured in milligrams per Liter (mg/L)
- NH4F ammonium measured in milligrams per Liter (mg/L) 
- NO2F - nitrite measured in milligrams per Liter (mg/L)
- NO3F - nitrate measured in milligrams per Liter (mg/L)
- NO23F - nitrite + nitrate measured in milligrams per Liter (mg/L)
- CHLA_N - chlorophyll a measured in micrograms per Liter (ug/L)
- NERR Site ID - ID given by NERR to identify the state where the sample was taken (NOC)
- Station Name - Full name of the station in which the sample was taken
- LatLong - coordinates in degrees of where the sample was taken
- Latitude in radians
- Longitudein radians
- Status of the monitoring station site the sample was from ("active" or "inactive")
- State in the U.S. where the sample was taken ("NC")
- Reserve Name - state of the U.S where the sample was taken ("North Carolina")
- Date in which the sample was collected

## Scripts and code

The Rmd file in the repository includes the code we used to conduct our study. It has the code for the inporting and wranggling of the raw data, the creation of the data sets we used in our study, and the creation of plots and figures to analyze the data. We did all of our analyses in R Studio in the Rmd file. 
