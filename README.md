# Energy-Center-of-Gravity
# Created by Jesse Barnett @ 6.07.2019 @ Center for Strategic and International Studies
# This repository contains four files:
# (1) Centroids_Data.csv contains the centroids (the coordiantes for the geometric center) of 244 countries, converted into degrees long/lat, raidans long/lat, and x-y-z coordinates in ECEF. It also contains long_converted, hyp, and lat_converted, which are used in the Haversine Formula. 
# (2) Energy_centers_Of_Gravity.csv is the "final" output file used by the visualization. It contains the outputed calculations of the "center of gravity" of a given commodity during a given year. This is calculated by taking the average of all 244 states' longitude and latitude coordinates (expressed in x,y,z ecef coordiantes) weighted by their share of the year's total production of a given energy commodity. To transform the 3 dimensional x,y,z ecef coordinates into 2 dimensional longitude latitute coordinates, I calculate the nearest surface coordinate. This is then converted into 2 dimensional longitude / latitude coordinates, and graphed as the center of gravity.
# (3) Oil Script Alpha is an r script that was used to assemble the underlying csvs. It may not be updated.
# (4) Raw_energy_Production_Data.csv, is a long format machine readable representation of each country's energy production (measured in MMBTU) by year and commodity, ranging from 1900 to 2014. 
# These files have also been compiled into a single Google Sheet, which can be accessed at https://docs.google.com/spreadsheets/d/1kb02oclNICmOTifLlQuzwh_kYC4U9Hmtx0whJnaKGzQ/edit?usp=sharing
# 
# About
# Raw data from # Raw data from http://www.tsp-data-portal.org/Energy-Production-Statistics#tspQvChart which is in turn compiled using data from Etemad & Luciani for the period 1900 - 1980, and the US EIA Historical Statistics for 1981 - 2013. 
