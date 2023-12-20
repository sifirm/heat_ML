# heat_ML
The context
Climate change is an urgent, relevant and mul3-dimensional global issue with a significant impact on energy policy and infrastructure. Tackling climate change involves both mi3ga3on (i.e. reducing greenhouse gas emissions) and adapta3on (i.e. preparing for the inevitable consequences). Mi3ga3ng greenhouse gas emissions requires changes to electricity systems, transport, buildings, industry and land use.
According to a report published by the Interna3onal Energy Agency (IEA), the life cycle of buildings, from construc3on to demoli3on, is responsible for 37% of global CO2 emissions linked to energy and processes in 2020. Yet it is possible to significantly reduce the energy consump3on of buildings by combining easy-to-implement solu3ons with cuMng-edge strategies. For example, renovated buildings can reduce hea3ng and cooling energy requirements by 50-90%. Many of these energy efficiency measures also deliver overall savings and other benefits, such as cleaner air for occupants. This poten3al can be achieved while maintaining the services provided by the buildings.
The dataset and challenge
It is clear that accurate predic3ons of energy consump3on for a given building as a func3on of its characteris3cs can help policy makers target renova3on efforts in order to maximise emissions reduc3ons.
The data we will be using comes from the Lawrence Berkeley Na3onal Laboratory (Berkeley Lab) and the work to be carried out consists of analysing differences in the energy efficiency of buildings in order to build one or more models to predict the energy consump3on of buildings.
To do this, the data provided describes the characteris3cs of the buildings and the clima3c and meteorological variables for the regions in which the buildings are located.
 Dataset description
The dataset contains approximately 100k observations collected over 7 years in different locations on building energy use.
The dataset includes building characteristics (e.g. floor area, type of installation, etc.), meteorological data for the building location (e.g. mean annual temperature, total annual precipitation, etc.) as well as energy consumption for the building and the given year,
Each line corresponds to a single building observed in a given year.
Your task is to predict the site EUI for each row, given the building characteristics and the meteorological data for the building location.
Evaluation metrics: root mean square error

 Features
id: building id
Year_Factor: anonymized year in which the weather and energy usage factors were observed
State_Factor: anonymized state in which the building is located : building classification
: building usage type
: floor area (in square feet) of the building
: year in which the building was constructed
: the energy star rating of the building : elevation of the building location
: minimum temperature in January (in Fahrenheit) at the location of the building
january_avg_temp: average temperature in January (in Fahrenheit) at the location of the building
january_max_temp: maximum temperature in January (in Fahrenheit) at the location of the building
cooling_degree_days: cooling degree day for a given day is the number of degrees where the daily average temperature exceeds 65 degrees Fahrenheit. Each month is summed to produce an annual total at the location of the building. heating_degree_days: heating degree day for a given day is the number of degrees where the daily average temperature falls under 65 degrees Fahrenheit. Each month is summed to produce an annual total at the location of the building. precipitation_inches: annual precipitation in inches at the location of the building
: annual snowfall in inches at the location of the building
: annual snow depth in inches at the location of the building
: average temperature over a year at the location of the building
: total number of days below 30 degrees Fahrenheit at the
location of the building
days_below_20F: total number of days below 20 degrees Fahrenheit at the location of the building
days_below_10F: total number of days below 10 degrees Fahrenheit at the location of the building
days_below_0F: total number of days below 0 degrees Fahrenheit at the location of the building
days_above_80F: total number of days above 80 degrees Fahrenheit at the location of the building
days_above_90F: total number of days above 90 degrees Fahrenheit at the location of the building
days_above_100F: total number of days above 100 degrees Fahrenheit at the location of the building
 State_Factor
 building_class
 facility_type
 floor_area
year_built
 energy_star_rating
 ELEVATION
 january_min_temp
      snowfall_inches
 snowdepth_inches
 avg_temp
 days_below_30F
       
days_above_110F: total number of days above 110 degrees Fahrenheit at the location of the building
direction_max_wind_speed: wind direction for maximum wind speed at the location of the building. Given in 360-degree compass point directions (e.g. 360 = north, 180 = south, etc.). direction_peak_wind_speed: wind direction for peak wind gust speed at the location of the building. Given in 360-degree compass point directions (e.g. 360 = north, 180 = south, etc.).
: maximum wind speed at the location of the building : number of days with fog at the location of the building
Target
• site_eui: Site Energy Usage Intensity is the amount of heat and electricity consumed by a building as reQlected in utility bills
Highlight what you have learned in the machine learning course by building a sklearn pipeline to:
- correctly pre-process the data according to its category (we don't give the steps to take into account here as they can be found in the different courses),
- choose the right hyper-parameters for the models selected (we don't give the hyper- parameters to look for here, as they have already been covered in the course).
An ini3al study of the data (EDA) is obviously necessary in order to understand the nature of each of the features.
CAUTION: if you use concepts that you have not seen in class, you must be able to understand and explain them. There is no point in copying code found on the Internet or generated by ChatGPT without understanding it. We much prefer a less extensive but perfectly understood piece of work to an exhaus3ve piece of work consis3ng of applying a set of techniques without understanding how they work or why they are useful.
To be handed in: a wri:en notebook (with comments) that you must present. This will have to jusAfy your choices for the different stages of the pipeline.
 • •
•
• •
  max_wind_speed
 days_with_fog
   Your job
