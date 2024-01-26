# Model bikeability
MSc Thesis: Traffic coverage quality by bike in Switzerland: A comparison of cities' bikeability


Each folder of the four case study areas Bern (BE), Lausanne (LS), Winterthur (WT) and Zurich (ZH) contains four files: One to preprocess the bike network, one to model cycling quality, one to model bikeability and one to model the change in bikeability based on bike infrastructures. With minor adaptions, particularly for the read in data, the scripts allow to reproduce the analysis to any other urban area in Switzerland. 

## Import of OSM data into PostgreSQL database
cyclosm_osm2pgsql.style: Style file to import data on bike infrastructures from OSM into PostgreSQL database with osm2pgsql
green_areas_osm2pgsql.style: Style file to import green areas from OSM into PostgreSQL database with osm2pgsql

## Preprocess network
BE_preprocess.Rmd, LS_preprocess.Rmd, WT_prerpocess.Rmd and ZH_preprocess.Rmd: Preprocessing of OSM line features to bike network

## Model cycling quality
BE_cycling_quality.Rmd, LS_cycling_quality.Rmd, WT_cycling_quality.Rmd and ZH_cycling_quality.Rmd: Model cycling quality of network segments using the type of bike infrastructure, the speed limit, the slope and green and aquatic areas

## Model bikeability
BE_bikeability.Rmd, LS_bikeability.Rmd, WT_bikeability.Rmd and ZH_bikeability.Rmd: Model bikeability with a gravity-based appraoch including previously modeled cycling quality

## Change in bikeability
BE_change_bikeability.Rmd, LS_change_bikeability.Rmd, WT_change_bikeability.Rmd and ZH_change_bikeability.Rmd: Change in mean distance to destinations considering BLOS compared to actual distance to isolate for the effect of bike infrastructure on bikeability

## Merge results of all four cities
Bikeability_all_cities.Rmd: Merge bikeability index values of all cities to one dataset for between-city comparison and mapping
Bikeability_change_all_cities.Rmd: Analyze change in mean distance for all four cities
