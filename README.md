# Temperature

## Overview:
This repository will contain all scripts used to clean and standardize the temperature data from autonomous logging devices installed in the Florida Keys and Dry Tortugas. The scripts will edit raw data from HoboWave, intermediate files, and master lists of all temperature data from all sites.

## Method:
CREMP has been monitoring corals along Florida’s Coral Reef since 1996. Every active CREMP monitoring site is now paired with a temperature logger. We currently have 77 loggers recording water temperatures from Martin County to the waters of Dry Tortugas National Park - 22 in Southeast Florida, 44 in the Florida Keys, and 11 in the Dry Tortugas. Our [Unified Florida Reef Map](https://myfwc.maps.arcgis.com/apps/webappviewer/index.html?id=ea7ac98649474cb9af7a6a20c823846d) is an ArcGIS map with multiple layers - to turn on the layer showing the temperature monitoring sites, click the “Show Contents of Map” icon on the left above “Unified Florida Coral Reef Tract Map”, then check the box next to “FRT Temperature Monitoring – CREMP Sites”.  We monitor water temperatures on a variety of different reef types and depths, including hardbottom habitats, shallow forereefs, deep forereefs, and patch reefs. 

Here is the current list of sites that have either historic or ongoing temperature data available:

[FWRI-Sites-with-Temperature-Data.pdf](https://github.com/user-attachments/files/24807796/temperature-table.pdf)

## Metadata:

| **Variable**                                | **Unit**                                                                 | **Description**
|-----------------------------------------|------------------------------------------------------------------------------|--------------------------------------------------------------------------|
| observation_id             | Integer                                                                        | Unique identifier for each individual observation that is recorded |
| date               | mm/dd/yyy       | The date the measurement was recorded on site |
| time               | Military standard time by hour      | The hour of that specific day that this observation was recorded |
| site_id             | Integer                                                                        | A unique indentifier assigned to each of the survey sites. The ID series is consistent through the Florida Key sites, Southeast Florida sites, and Dry Tortugas National Park. |
| site_name              | Text       | The name of the location where the surveys occur and where sensors are located (survey sites) |
| temp_C             | Degrees Celsius (°C)                                                                         | Recorded via autonomous devices placed on site that sample once per hour. Devices are removed off site when data is collected, and immediately replaced with another to prevent gaps in sampling. Devices are read through HoboWare, and results are saved as .xls or .csv files|
| temp_F             | Degrees Fahrenheit (°F) | Converted from the recorded temperature in Celsius|


