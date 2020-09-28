# Dissertation
This repository contains modified fortran code for running the Weather Research and Forecasting Model v 4.0. The model has been modified to include methods for irrigation in the land surface model.

The file namelist.input section &physics has an added irrigation parameter opt_irrig. This parameter has a default of 0, which is apply no irrigation, and only works for the Noah land surface model with mosaic option and the Noah-MP model. Running WRF using another land surface model such as CLM will not use this parameter.

Link to dissertation: 
