# CE6800 Term Project - EWBGWU Bhutiya Water Management Program Collaboration
This project is in support of the Engineers Without Borders GWU Bhutiya Water Management Program, in their aim to combat climate change-driven water scarcity, over-exploitation of groundwater resources, and inefficient irrigation practices.

This project will inform the design process for an integrated dam-percolation pond system for the Bhutiya community. This code seeks to estimate expected rainfall, runoff conversion, and thereby the optimal dimensions and design of the proposed system.

# Progress Report Notes

Phase I Notes (Olivia):
   The team’s project is a three-phase project and each phase has specific inputs and outputs. Sophia and I are working on Phase 1, the precipitation prediction model using time series analysis. I have found precipitation data for East and West Rahjastan, temperature data, and other independent variables that could be used in our model. I have contributed to the team’s literature review, investigating various climate models, the necessary variables, and noting how this research will ultimately aid in creating our model. Throughout this process, I looked at both the modelling methods as well as sources of data. Our team faced the obstacle of obtaining complete and specific data for climate variables for the correct time frame to use as independent variables. I currently in the process of downloading WeatherUnderground data since this service has a summary of climate statistics daily and monthly.<br /> 
   Other preliminary work includes cross validation modelling as well as ensemble method and pipelines to help understand the precipitation data. These models used techniques from CE6800 lessons and expanded upon them. The continuous variable of precipitation was changed to a binary variable based on the month’s precipitation value compared to that month’s average precipitation value for the time range of our data. These models are not as helpful as time series analysis in regard to predicting a continuous variable. I have also used visualization methods to better understand the data, including seaborn, matplotlib, and plotly. I am currently in the process of visualizing the anomalies for temperature and precipitation. <br /> 
 

Phase II Notes (Sophia):
	In order to properly size the dam and catchment system (Phase III) given expected rainfall (Phase I), the expected precipitation must be converted to runoff. The catchment yield of the system will be a function of direct runoff dependent on the basic watershed hydrology. The system will not collect the total amount of rainfall falling over the draining area. Instead, catchment yield will be controlled by factors of evaporation, infiltration, depression storage, and canopy interception (to name a few). In equation form the water balance approach looks like this:

Streamflow Q = Precipitation P -  (Transpiration+Evaporation) T - Infiltration I - Soil Storage S	

Based on preliminary analysis and literature review, it may be necessary to perform Thiessien Polygon or Isohyetal methods of hydraulic modeling to understand how rainfall affects sub-watersheds within the drainage area. Numerous softwares are available online including HEC-HMS and SWAT are currently being investigated as tools to simulate the quality and quantity of surface and ground water and predict the environmental impact of land use, land management practices, and climate change.

For the first iteration of the hydraulic model a simple equation was adapted from the Australian Agricultural Ministry (1). 
Catchment Yield (litres) = Catchment Area (hectares) x Annual Rainfall (mm) x Yield Coefficient

Phase III Notes (Tom)
	With the volume of runoff from phase II, as well as the data obtained from google we will be able to utilize code in order to dimension the anicut structure. We will be able to determine the height at which the dam needs to be in order to retain the water, and through the height determine the length of the dam. With the length and height of the dam our team should be able to determine the full dimensions of the dam. Once the anicut structure has been designed, the area of the pond behind the dam can be fully designed, knowing both the maximum height at which the pond can rise, and the full width at which the pond can spread. 
	Phase III involves the use of equations, and functions in order to determine the dimensions of the percolation pond, anicut system. The first task will be to find the maximum runoff within the given range of years. This maximum runoff will allow the team to develop a percolation pond that can handle the largest inflow of water. 


References:

(1) Farm Water Calculator: Determining Catchment Yield for Planning Farm Dams. (n.d.). Retrieved April 5, 2020, from http://calculator.agriculture.vic.gov.au/fwcalc/information/determining-catchment-yield-for-planning-farm-dams

(2) Jasrotia, A. S., Majhi, A., & Singh, S. (2009). Water balance approach for rainwater harvesting using remote sensing and GIS techniques, Jammu Himalaya, India. Water resources management, 23(14), 3035-3055. Retrieved April 5, 2020.


