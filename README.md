# MTA-Daily-Ridership

## Problem Statement 
-The MTA (Metropolitan Transportation Authority) is the public transportation agency responsible for managing and operating transit systems in the New York City metropolitan area. This includes the New York City subway and bus systems, as well as commuter rail services like Long Island Rail Road and Metro-North. The MTA also oversees bridges and tunnels in the city. MTA services the five boroughs and also commutes to some areas upstate and New Jersey. This data can be used to capture the estimated total ridership of different forms of MTA Transportation before, during and after the COVID-19 Pandemic. 

-The purpose of this analysis is to illustrate how busy MTA transportation is in NYC. We can get an idea of what modes of transportation are most used, around what times they are most buisiest and can attribute the reason to why this may be. This data can also help one determine whether they want to use public transportaion or use their own personal vehicle. This way they can weigh the pros and cons.

## Data Dictionary
Include a data dictionary to explain the meaning of each variable or field in the dataset.

Column Name                                Description                                         API Field Name                           Data Type    
-------------------------------------------------------------------------------------------------------------------------------------------------------------
-Date                                       The date of travel (MM/DD/YYYY).                    date                                     Floating Timestamp

-Subways: Total Estimated Ridership         The daily total estimated subway ridership.         subways_total_estimated_ridership        Number

-Subways: % of Comparable Pre-Pandemic Day  The daily ridership estimate as a percentage of subway ridership on an equivalent day prior to the COVID-19 pandemic.                                                                                      subways_of_comparable_pre_pandemic_day   Number

-Buses: Total Estimated Ridership           The daily total estimated bus ridership.            buses_total_estimated_ridersip           Number

-Buses: % of Comparable Pre-Pandemic Day    The daily ridership estimate as a percentage of bus ridership on an equivalent day prior to the COVID-19 pandemic.                                                                                                buses_of_comparable_pre_pandemic_day     Number

-LIRR: Total Estimated Ridership            The daily total estimated LIRR ridership. Blank value indicates that the ridership data was not or is not currently available or applicable.                                                              lirr_total_estimated_ridership          Number

-LIRR: % of Comparable Pre-Pandemic Day     The daily ridership estimate as a percentage of LIRR ridership on an equivalent day prior to the COVID-19 pandemic.                                                                                       lirr_of_comparable_pre_pandemic_day     Number

-Metro-North: Total Estimated Ridership     The daily total estimated Metro-North ridership. Blank value indicates that the ridership data was not or is not currently available or applicable.                                                              metro_north_total_estimated_ridership   Number

-Metro-North: % of Comparable Pre-Pandemic Day The daily ridership estimate as a percentage of Metro-North ridership on an equivalent day prior to the COVID-19 pandemic.                                                                                    metro_north_of_comparable_pre_pandemic_day Number

-Access-A-Ride: Total Scheduled Trips       The daily total scheduled Access-A-Ride trips. Blank value indicates that the ridership data was not or is not currently available or applicable.                                                              access_a_ride_total_scheduled_trips      Number

-Access-A-Ride: % of Comparable Pre-Pandemic Day   The daily total scheduled trips as a percentage of total scheduled trips on an equivalent day prior to the COVID-19 pandemic.                                                                              access_a_ride_of_comparable_pre_pandemic_day   Number

-Bridges and Tunnels: Total Traffic         The daily total Bridges and Tunnels traffic.         bridges_and_tunnels_total_traffic         Number

-Bridges and Tunnels: % of Comparable Pre-Pandemic Day    The daily total traffic as a percentage of total traffic on an equivalent day prior to the COVID-19 pandemic.                                                                                       bridges_and_tunnels_of_comparable_pre_pandemic_day
                                                                                                                                          Number
-Staten Island Railway: Total Estimated Ridership   The daily total estimated SIR ridership.    staten_island_railway_total_estimated_ridership   Number

-Staten Island Railway: % of Comparable Pre-Pandemic Day   The daily ridership estimate as a percentage of SIR ridership on an equivalent day prior to the COVID-19 pandemic.                                                                             staten_island_railway_of_comparable_pre_pandemic_day    Number


## Executive Summary

### Data Cleaning Steps
While viewing the data I noticed there was a date column which contained the month, day of the month and year in number form. Since I wanted to complete analysis for each of these I created a function that extracted the month, day of the month and year and created a column for Month, Year and Day of Week using (dt) dateeime functions. This changed the dtypes for month and day of week to objects making it easier to use within my analysis. 

### Key Visualizations
Include key visualizations that highlight important aspects of the data. Use graphs, charts, or any other visual representation to make your points.