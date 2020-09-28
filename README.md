# Dissertation
This repository contains modified fortran code for running the Weather Research and Forecasting Model v 4.0. The model has been modified to include methods for irrigation in the land surface model.

The file namelist.input section &physics has an added irrigation parameter opt_irrig. This parameter has a default of 0, which is apply no irrigation, and only works for the Noah land surface model with mosaic option and the Noah-MP model. The land use categories must be based on USGS 24 category data, in particular irrigated cropland must be designated as category '3'. Running WRF using another land surface model such as CLM will not invoke this parameter.

opt_irrigate = 1,

Set top two soil layers to field capacity at each time step if less than field capacity. If using Noah:Mosaic, it only performs these steps for the fraction of the gridc cell. In Noah-MP, applies to entire grid cell if dominant land use category is irrigated cropland. 

opt_irrig = 2,


Link to dissertation: 
