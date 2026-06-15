# Dataset Description: King et al. “Spatial Co-Variability between Bedrock-to-Canopy Structure and Soil Texture Reveal Patterns of Growing-Season Soil Moisture Persistence across a Rocky Mountain Watershed”

## 1. Geospatial Data Layers

All data layers, with the exception of predicted clay and sand content, are derived from previously published datasets, and are described in the supplemental data of King et al. All rasters are resampled to 10 m resolution. Topographic variables were computed using the DEM and TopoToolBox (Schwanghart & Scherler, 2014). 

The geospatial data layers are hosted externally: [Data](https://drive.google.com/drive/folders/1oDRfgWEceTJ81bIF61zWmvgOiuNJnf9P?usp=sharing)

| Data layer | Description | Filename |
| :---- | :---- | :---- |
| Predicted clay % | | pred\_clay.tif |
| Predicted sand % | | pred\_sand.tif |
| POLARIS Clay % | Probability-weighted expected values across all the soil series predicted for each pixel, from Chaney et al. (2016; 2019). Values are averaged across depth intervals of 0–5 and 5–15 cm. | clay\_polaris.tif |
| POLARIS Sand % | Probability-weighted expected values across all the soil series predicted for each pixel, from Chaney et al. (2016; 2019). Values are averaged across depth intervals of 0–5 and 5–15 cm. | sand\_polaris.tif |
| Geology | From CO geologic map (Green, 1992). | co\_geol.zip |
| Distance to intrusive rock contact | Euclidean distance from each pixel to the nearest intrusive rock contact, with negative values indicating locations within the formation. | intrusive.tif |
| Distance to shale rock contact | Euclidean distance from each pixel to the nearest shale rock contact, with negative values indicating locations within the formation. | shale.tif |
| NDVI | Peak NDVI from 2021, using  Landsat 8 imagery (USGS, 2021). | ndvi.tif |
| Elevation | DEM (USGS, 2024\) | elevation.tif |
| Potential incoming solar radiation | Annual net potential solar radiation, based on Hebeler (2016) and Kumar et al. (1997).  | radiation.tif |
| HAND | Height above nearest drainage, computed as the elevation difference to the nearest downstream channel pixel, which approximates water table depth (Rennó et al., 2008).  | hand.tif |
| TWI | Topographic Wetness Index | twi.tif |
| Slope |  | slope.tif |
| Stream | Stream location as delineated using DEM and TopoToolBox (Schwanghart & Scherler, 2014).  | stream.zip |

## 2. Sampling Locations

### Soil texture sampling locations (*soil\_texture.csv*)

This dataset includes 303 core locations as collected at 2.5–7.5 cm depth during the 2018 National Ecological Observatory Network's Airborne Observation Platform (NEON AOP) campaign (Chadwick et al., 2020). 13 additional cores were collected at 10 cm depth during 2021 and 2023 field campaigns. All sample materials \< 2 mm were analyzed using the hydrometer method to determine fractional clay and sand content (Huluka and Miller, 2014). Clay and sand content are included as attributes.

### Soil moisture sensor locations (*soil\_moisture.csv*)

This dataset shows the locations of 36 soil moisture sensors. The sensors are high-frequency (15-minute interval) TMS-4 loggers, which record raw counts proportional to volumetric water content, integrated over the upper 0–10 cm of soil (Wild et al., 2019). Two soil moisture metrics, *mean* and *b*, are included as attributes. *Mean* refers to the 2022 growing-season mean soil moisture recorded at each sensor, and *b* refers to the mean growing-season exponential depletion rate following growing-season rainfall events. Descriptions of these metrics are reported in King et al.

References:

Chadwick, K. D., Pierce, S., Sirles, M., Lawrence, C., Cullen, J., Grant, K., Falco, N., Maher, K., & Dafflon, B. (2020). Soil bulk density and texture data collected during field survey associated with NEON AOP survey, East River, CO 2018 \[Data set\]. ESS-DIVE.

Chaney, N. W., Wood, E. F., McBratney, A. B., Hempel, J. W., Nauman, T. W., Brungard, C. W., & Odgers, N. P. (2016). POLARIS: A 30-meter probabilistic soil series map of the contiguous United States. Geoderma, 274, 54-67.

Chaney, N. W., Minasny, B., Herman, J. D., Nauman, T. W., Brungard, C. W., Morgan, C. L. S., McBratney, A. B., Wood, E. F., & Yimam, Y. (2019). POLARIS soil properties: 30-m probabilistic maps of soil properties over the contiguous United States. Water Resources Research, 55(4), 2916–2938.

Green, G. N. (1992). The digital geologic map of Colorado in ARC/INFO format (Open-File Report 92–0507). U.S. Geological Survey.

Hebeler, F. (2016). Solar radiation modeling for complex topography using GIS \[Master’s thesis, University of Zurich\].

Huluka, G., & Miller, R. (2014). Particle size determination by hydrometer method. In F. J. Sikora & K. P. Moore (Eds.), Soil test methods from the southeastern United States (Southern Cooperative Series Bulletin 419, pp. 180–184). University of Georgia.

Kumar, L., Skidmore, A. K., & Knowles, E. (1997). Modelling topographic variation in solar radiation in a GIS environment. International Journal of Geographical Information Science, 11(5), 475–497.

Rennó, C. D., Nobre, A. D., Cuartas, L. A., Soares, J. V., Hodnett, M. G., & Tomasella, J. (2008). HAND, a new terrain descriptor using SRTM-DEM: Mapping terra-firme rainforest environments in Amazonia. Remote Sensing of Environment, 112(9), 3469-3481.

Schwanghart, W., Scherler, D. (2014): TopoToolbox 2 – MATLAB-based software for topographic analysis and modeling in Earth surface sciences. Earth Surface Dynamics, 2, 1-7.

U.S. Geological Survey (USGS) (2021). Landsat 8 (L8) Data Users Handbook. U.S. Geological Survey.

U.S. Geological Survey (USGS) (2024). 3D Elevation Program (3DEP) 10-meter resolution digital elevation model (1/3 arc-second) \[Data set\]. U.S. Geological Survey.

Wild J., Kopecký M., Macek M., Šanda M., Jankovec J., & Haase T. (2019) Climate at ecologically relevant scales: A new temperature and soil moisture logger for long-term microclimate measurement. Agricultural and Forest Meteorology, 268, 40–47.
