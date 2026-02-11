# Temperature

## Overview:

This repository will contains all scripts used to clean and standardize the Coral Research Program's temperature data from autonomous logging devices installed in Southern Florida, the Florida Keys, and Dry Tortugas National Park. The scripts will edit raw temperature data from HoboWare (in the form of csv files), intermediate temperature products, and master lists of all observations in a given year from all sites or a selection thereof.

## The Program:

The Coral Reef Evaluation & Monitoring Program (CREMP) has been monitoring corals in Florida's coastal waters since 1996. Every active CREMP monitoring site is now paired with a temperature logger. We currently have 77 loggers recording water temperatures from Martin County to the waters of Dry Tortugas National Park - 22 in Southeast Florida, 44 in the Florida Keys, and 11 in the Dry Tortugas.

Our [Unified Florida Reef Map](https://myfwc.maps.arcgis.com/apps/webappviewer/index.html?id=ea7ac98649474cb9af7a6a20c823846d) is an ArcGIS map with multiple layers that will allow you to explore our monitoring sites. To turn on the layer showing the temperature monitoring sites, click the “Show Contents of Map” icon on the left above “Unified Florida Coral Reef Tract Map”, then check the box next to “FRT Temperature Monitoring – CREMP Sites”.  We monitor water temperatures on a variety of different reef types and depths, including hardbottom habitats, shallow forereefs, deep forereefs, and patch reefs.

Here is the current list of sites that have either historic or ongoing temperature data available:

[FWRI-Sites-with-Temperature-Data.pdf](https://github.com/user-attachments/files/24807796/temperature-table.pdf)

## Metadata:

| **Variable** | Data Type/Unit | **Description** |
|----|----|----|
| observation_id | Integer | Unique identifier for each individual observation that is recorded |
| date | Date (yyyy-mm-dd) | The date the measurement was recorded on site |
| time | HMS object (standard military time/ 00:00:00) | The time of day that the measurement was recorded on site |
| site_id | Integer | A unique identifier assigned to each of the survey sites. The ID is serial through the Florida Key sites, Southeast Florida sites, and Dry Tortugas National Park. |
| site_name | Character | The name of the location where the surveys occur and where sensors are located (survey sites) |
| temp_C | Numeric (degrees Celsius/°C) | The temperature recorded by the device |
| temp_F | Numeric (degrees Fahrenheit/°F) | Converted from the recorded temperature in Celsius |

## Procedure:

As of 2026, sensors sample at a rate of 1 observation per hour. Devices are removed from site when data is collected, and immediately replaced with another to prevent gaps in sampling. Devices are read through HoboWare, and results are saved as .csv files
