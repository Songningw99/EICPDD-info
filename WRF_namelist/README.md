# WRF namelist examples
1. For GCMs: The WRF intermediate files are generated with [Pywinter](https://github.com/dniloash/Pywinter) from NetCDF datasets. So no ungrib section in WPS namelist. 
2. For ERA5: The WRF intermediate files are generated from GRIB files. The upper level data and surface data are stored in different GRIB files so ungrib need to run twice for both type of data. The ERA5 data we used is on model level, so the PRES data need to be generated before running metgrid.exe. 
3. The simulation domain is centered at the centroid of the selected potential convection case. 