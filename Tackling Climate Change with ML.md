# Abstract

This paper discusses how ML can be used to reduce GHG emissions and help society adapt to changing climate. It flags the proposed solutions into levels of implement-ability based on current technology trends as : 
1. High leverage : bottlenecks that are best suited to be solved by ML
2. Long term : Applications that will have their primary impact after 2040. 
3. Uncertain impact : Impact on GHG emissions is uncertain. 

# Buildings and Cities

Energy consumed in buildings is responsible for a quarter of global energy-related emissions. [@moraGlobalRiskDeadly2017]  [@moraTwentySevenWaysHeat2017] describe the health risks associated with exposure to heat that exceeds human thermoregulatory capacity. 

[@avandUsingMachineLearning2021] used LANDSAT versions 5,7,8 to model flooding in susceptible areas.

[@kolterLargeScaleStudyPredicting2011] collected monthly electricity and gas bills from local utility company, coupled that with GIS database to model end user energy consumption.   

[@geissRemoteSensingBasedCharacterization2011] clustered buildings into types to assess the potential of district heat in a German town

[@luBuildingTypeClassification2014], [@hennAutomaticClassificationBuilding2012], [@BreakingNewGround2017] used remote sensing to infer infrastructure data and mapping human settlements.

## DataSets

|DOI|Source|Data|Algorithms|Remarks|
|--|----------------------|----------------------|----------------------|----------------------|
|10.1038/nclimate3322<br/>|[Government Websites](#earth-system-models)|<ol><li> daily mean near-surface wind speed </li> <li> daily mean near-surface relative humidity </li> <li>daily mean/min/max near-surface air temperature</li></ol>|<ol><li>[[Support Vector Machines]] with 16 variables to discriminate climate conditions between hot days and cold days</li></ol>|Model with mean daily relative humidity and mean daily surface air temperature yielded highest relative accuracy of any two pairs of variables| 
|10.1016/j.jhydrol.2020.125663|1990-2019 earthexplorer.usgs.gov, search.asf.alaska.edu for landsat(5,7,8) imagery TM and OLI sensors to create LULC maps  |Raster images with 30m resolution|For flood susceptibility mapping<ol><li>[[Random Forest]]</li><li>[[Bayesian Generalized linear models]]</li></ol>|ROC and kappa coefficient were used to validate the models|
|10.1609/aaai.v25i1.7806|<ol> <li>[Cambridge GIS](http://www.cambridgema.gov/gis.aspx)</li><li>[Tax assessor records](http://www2.cambridgema.gov/fiscalaffairs/PropertySearch.cfm)</li><li>NStar</li><ol>|Electricity gas bills with corresponding street addresses|<ol><li>[[Linear Regression]]</li><li>[[Gaussian Process Regression]]</li></ol>|
|10.3390/rs3071447||<ol><li>Digital Surface Model</li><li>multispectral IKONOS imagery</li><li>Landsat and  SAR from TerraSAR-X data</li><li>OSM</li></ol>|[[EM expectation maximization]]|
|10.1016/j.landurbplan.2014.07.005|<ol><li>Sanborn Map Company</li><li>Denver GIS center</li></ol>|<ol><li>Lidar Data 1064nm 50kHz</li><li>Land Parcel polygons 200m</li></ol>|<ol><li>[[Support Vector Machines]]</li><li>[[Aggregated Decision Tree]]</li><li>[[Random Forest]]</li></ol>|50-50 split for calibration and validation and 10% minority class data points|


### Supplementary Images
#### Earth System Models
![Datasets for surface properties](govt-meteorological-datasets.png)
