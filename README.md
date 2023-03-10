# Project Chelanigans
Assessing temporal variability in littoral algae (or glacial till) at Lake Chelan, WA   

## Project Title: Assessment of temporal variability in littoral algae (or glacial till) at Lake Chelan, WA  

## Team: Jason MacDonald  

## Short summary  
This study will attempt to quantify the abundance of littoral algae along the shore of Lake Chelan and track any patterns over the past ~50 years to develop a better understanding of how much change has occurred.  

## Background  
Filamentous algae in the littoral region of Lake Chelan have become a concern in recent years. The filamentous algae attaches to rocks along the shoreline and is viewed as a nuisance organism to property owners and visitors. Oligotrophic lakes, like Lake Chelan, are characterized by low nutrients and limited algal growth. The appearance of littoral filamentous algae in an oligotrophic lake is commonly associated with an increased flux of nutrients such as Nitrogen and Phosphorus. Currently, there is no ongoing data collection occurring at Lake Chelan regarding littoral algae and previous experiments are sparse.   

alternative:  
Global climate change has caused rapid melting of glaciers, including those which feed into Lake Chelan. As glaciers melt, the turbidity caused by glacial till can be tracked by satelite imagery. Glacial till is composed of inorganic material that is void of nutrients and creates an impermeable layer on the lakebed. Glacial till has also been shown to have negative effects on plankton [6].  

## Objectives  
1. Identify temporal trends in benthic algae coverage (south half of lake)   
2. Identify temporal trends in glacial till turbidity (north half of lake)   

## Datasets  
Sentinel-2  
https://cloud.google.com/storage/docs/public-datasets/sentinel-2#dataset_access    
base URL https://storage.googleapis.com/gcp-public-data-landsat/LC08/01  

Harmonized Landsat-8 & Sentinel-2 (HLS)
https://cmr.earthdata.nasa.gov/cloudstac/LPCLOUD
https://gist.github.com/scottyhq/efd583d66999ce8f6e8bcefa81545b8d
  
    
## Tools and packages  
1. Rasterio  
https://rasterio.readthedocs.io/en/latest/api/rasterio.html  
2. Numpy  
https://numpy.org/  
3. Pandas  
https://pandas.pydata.org/  
4. GeoPandas  
https://geopandas.org/  
5. Shapely  
https://pypi.org/project/Shapely/  
6. SeaDAS
https://seadas/gsfc/nasa.gov/

## Planned methodology/approach  
* Phase 1
    1. Develop script to access all relevant HLS data from NASA  
    2. Filter images with more than 10% cloud cover  
    3. Adjust window extents
* Phase 2    
    1. Find correct rgb/nir ratios to identify benthic algae (or glacial till with alternative)  
    2. Develop a notebook that will track temporal changes in abundance (area) and/or intensity  
    3. Create a timeseries to visualize seasonal and annual changes since 2016  

## Expected outcomes  
1. Visualize the apparent increase in benthic algae 
2. Visualize seasonality in glacial till  

## Conclusions, Results and Lessons Learned  

## Future Work  

## Any other relevant information, images/tables, references, etc.  

## References  

[1]
Jean M. Jacoby, Debra D. Bouchard & Clayton R. Patmont "Response of Periphyton to Nutrient Enrichment in Lake Chelan, WA," Lake and Reservoir Management, 7:1, 33-43, 1991, DOI: 10.1080/07438149109354252

[2]
M. Reif, B. Krumwiede, S. Brown, E. Theuerkauf, and J. Harwood, “Nearshore Benthic Mapping in the Great Lakes: A Multi-Agency Data Integration Approach in Southwest Lake Michigan,” Remote Sensing, vol. 13, no. 15, p. 3026, Aug. 2021, doi: 10.3390/rs13153026.

[3]
C. J. Legleiter and S. W. Hodges, “Mapping Benthic Algae and Cyanobacteria in River Channels from Aerial Photographs and Satellite Images: A Proof-of-Concept Investigation on the Buffalo National River, AR, USA,” Remote Sensing, vol. 14, no. 4, p. 953, Feb. 2022, doi: 10.3390/rs14040953.

[4]
C. Baughman, B. Jones, K. Bartz, D. Young, and C. Zimmerman, “Reconstructing Turbidity in a Glacially Influenced Lake Using the Landsat TM and ETM+ Surface Reflectance Climate Data Record Archive, Lake Clark, Alaska,” Remote Sensing, vol. 7, no. 10, pp. 13692–13710, Oct. 2015, doi: 10.3390/rs71013692.

[5]
Jassby, Alan D., Goldman, Charles R., Reuter, John E., Richards, Robert C., "Origins and scale dependence of temporal variability in the transparency of Lake Tahoe, California–Nevada," Limnology and Oceanography, 2, 1999, doi: 10.4319/lo.1999.44.2.0282.

[6]
Sommaruga, R., Kandolf, G. "Negative consequences of glacial turbidity for the survival of freshwater planktonic heterotrophic flagellates." Sci Rep 4, 4113 (2014). https://doi.org/10.1038/srep04113

[7]
Laird, K.R., Barouillet, C., Cumming, B.F. et al. "Influence of glacial turbidity and climate on diatom communities in two Fjord Lakes (British Columbia, Canada)." Aquat Sci 83, 13 (2021). https://doi.org/10.1007/s00027-020-00767-3

[8]
Martin Claverie, Junchang Ju, Jeffrey G. Masek, Jennifer L. Dungan, Eric F. Vermote, Jean-Claude Roger, Sergii V. Skakun, Christopher Justice, "The Harmonized Landsat and Sentinel-2 surface reflectance data set." Remote Sensing of Environment, Volume 219, 2018, Pages 145-161, ISSN 0034-4257, https://doi.org/10.1016/j.rse.2018.09.002. (https://www.sciencedirect.com/science/article/pii/S0034425718304139)

[9]
Harmonized Landsat-8 Sentinel-2 (HLS) Product User's Guide
https://hls.gsfc.nasa.gov/wp-content/uploads/2017/08/HLS.v1.3.UserGuide_v2-1.pdf

[10]
Overview of sentinel-2
https://sentinels.copernicus.eu/web/sentinel/user-guides/sentinel-2-msi/overview

[11]
Hossain, AKM & Jia, Yafei & Chao, Xiaobo. (2010). Development of Remote Sensing Based Index for Estimating/Mapping Suspended Sediment Concentration in River and Lake Environments. 