# Final Project Part 3: Data Processing, Setbacks, and a Website
[Back to Part 1](kelp-proj-HNeblina.md)

[Back to Part 2](final-part-2)

[Back to Portfolio](README.md)

[My Kelp Website](https://carnegiemellon.shorthandstories.com/070951e8-c3d6-49d9-8166-4a097fa5b8f1/index.html)

## Big Data is a Big Hassle
The most interesting data I used for this project was a collection of 30 by 30 meter raster cells tracking kelp forest biomass for the entire US West Coast, as well as a big chunk of the Pacific Ocean. When I first found these data, I was releived--it was just what I needed. 

However, it was not easy to handle. To start, the file size was so large that it took over an hour just to download the data, though it was no surprise that such an expansive swath of satellite imagery would be cumbersomely large. What was more of an obstacle was the file type: NetCDF. I had never seen it before, let alone used it in a project. After doing some research, I learned two things. First, NetCDF files for this type of imagery usually held time-series raster data, exactly what I hoped for. Second, they were a hassle to use in general and specifically in ArcGIS Pro, where I intended to make a large portion of my visualizations.

I tried to use the raster data as intended. I imported it into my project, and I tried to make a mosaic data set that contained information on each year--over and over again. One of the tools in ArcGIS ran for seven and a half hours. It failed. After what must have been at least a dozen hours of failed geoprocessing, I took the advice of my professor, Dr. Goranson, and tried to convert the NetCDF rasters to points. That failed, too. However, I did manage to extract the information as a table (on the second or third try), and I knew I could 
