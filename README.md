# Processing Large Satellite Image Collections as Data Cubes with the gdalcubes R package


*Workshop materials for OpenGeoHub Summer School 2019*

Analyzing large collections of satellite imagery is inherently complex: images may spatially overlap, may have different spatial reference systems, and spectral bands may be recorded at different spatial resolutions. To make practical use of multispectral and multitemporal imagery, possibly combining datasets from different Earth observation missions, data scientists rather require a regular data structure such as a data cube. The R package gdalcubes can build regular raster data cubes from satellite image collections on-the-fly, without the need to maintain a second copy of the data. Users define the geometry of the cube and a chain of data cube operations and let gdalcubes take care of reprojection, rescaling, resampling, and cropping. The package furthermore organizes tiling and parallelization.

The tutorial will introduce the basic concepts and usage of the R package, demonstrating how raster data cubes can be created and processed. In the demonstration part, we will look in detail at the parameters of data cubes and available operations. We will process different datasets e.g. from the Sentinel-2, Landsat 8, and MODIS missions with size up to a few hundred gigabytes. In the practical part, participants work on smaller exercises using a downsampled Landsat 8 time series, covering a small part of the Brazilian Amazon forest.

## Installation Instructions 

1. Install R and the following packages from CRAN: `install.packages(c("gdalcubes", "magrittr", "raster", "stars", "mapview", "viridis"))`

2. Download and unzip the sample dataset for the practical part from https://uni-muenster.sciebo.de/s/e5yUZmYGX0bo4u9/download.


## Links

- [Slides]() of plenary presentation
- [Workshop Notebook](https://appelmar.github.io/opengeohub_summerschool2019/tutorial.html)
- [Exercise Solutions](https://github.com/appelmar/opengeohub_summerschool2019/blob/master/solutions.R)




## References

- https://www.r-spatial.org/r/2019/07/18/gdalcubes1.html

- Appel, M., & Pebesma, E. (2019). On-Demand Processing of Data Cubes from Satellite Image Collections with the gdalcubes Library. Data, 4(3), 92. https://doi.org/10.3390/data4030092

