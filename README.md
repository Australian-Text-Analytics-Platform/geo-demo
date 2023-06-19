# Tools for geolocation

These tools will retrieve location information for placenames and plot the placenames on a map using the location information. Two databases of location information are demonstrated, the  [OpenStreetMap Geocoder API](https://geocoder.readthedocs.io/providers/OpenStreetMap.html) and the [TLC Gazetteer of Historical Australian Places](https://tlcmap.org/help/guides/ghap-guide/#ws).

To use the notebooks, first prepare a CSV file with a list of placenames, with a column header name `LocationName` and one name per row (see example below). Save it as `placenames.csv`. 

```csv
LocationName
Brisbane
Caloundra
Melbourne
Adelaide
```

## Running the geocoding tools

### OpenStreetMap Geocoder API

1.1. To search the global OSM database, start the OSM notebook. You will need to sign in to use the ATAP Binder using CILogon authentication. You can use your institutional, Google or Microsoft account to login.

[![Binder](https://binderhub.atap-binder.cloud.edu.au/badge_logo.svg)](https://binderhub.atap-binder.cloud.edu.au/v2/gh/Australian-Text-Analytics-Platform/geo-demo/main?labpath=geo_demo_osm.ipynb)

1.2. A sample CSV file of placenames is included with the notebook, or you can upload your own. If your data file is named differently you will need to change the filename in the notebook code.

1.3. Run the code cells to search OSM for the provided placenames.


### TLC Gazetteer
2.1. To search the TLC database, run the code in the TLC notebook. Note that the TLC database is of Australian placenames only, and can return multiple results for each name.

[![Binder](https://binderhub.atap-binder.cloud.edu.au/badge_logo.svg)](https://binderhub.atap-binder.cloud.edu.au/v2/gh/Australian-Text-Analytics-Platform/geo-demo/main?labpath=geo_demo_tlc.ipynb)


### Map

3.1. When the code in either geocoding notebook has completed, a new file named `geocoded-data.csv` will be created alongside the notebook. Download this if you want to keep a copy of it. 
3.2. After running one of the OSM or TLC notebooks, run the code in the map notebook. 

[![Binder](https://binderhub.atap-binder.cloud.edu.au/badge_logo.svg)](https://binderhub.atap-binder.cloud.edu.au/v2/gh/Australian-Text-Analytics-Platform/geo-demo/main?labpath=geo_demo_map.ipynb)


