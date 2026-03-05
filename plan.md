

## Steps

Download and clip SNODAS raster to Steamboat Springs boundary.
Fetch OSM building footprints for that boundary.
Fetch FEMA flood zone polygons for that boundary.
Filter buildings to only those inside flood zones.
Sample SWE values from the raster onto those buildings.
Create a vulnerability score (what factors feed into this?).
Export and map.

## Beginning
Write a Python script that:

Uses OSMnx to fetch the Steamboat Springs city boundary - DONE
Checks the length of the resulting GeoDataFrame - DONE 
Checks the geometry type(s) - DONE
Prints the bounds - DONE
Creates a quick Folium map to visualize it - DONE

## SWE Notes
Steamboat Springs, CO resides in the Upper Yampa Subbasin.
Nearby SNOTEL station is 'Dry Lake'
According to below graphs, Median Peak SWE is April 6-8. This year (2026) is a much lower year for SWE than years prior. Finding a year with at/above median SWE value.

Aiming for April 12, 2024 dataw

 https://nwcc-apps.sc.egov.usda.gov/awdb/basin-plots/POR/WTEQ/assocHUC8/14050001_Upper_Yampa.html?showYears=2026

 https://nwcc-apps.sc.egov.usda.gov/awdb/site-plots/POR/WTEQ/CO/Dry%20Lake.html?showYears=2026

 SNODAS User Guide: https://nsidc.org/sites/default/files/g02158-v001-userguide_2_1.pdf
 