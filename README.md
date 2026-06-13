# Earth-211-Final-Project
An Earth Science data analysis project

#Final Project Submission
An analysis of how metal concentration varies with energy use type both in the form of a time series and by state. Final report is in the "Final Report" section. All parts of the final report are summarized or include more detail in the individual sections. Result summaries are in the results section, final figures and tables are in figures and tables, and references are in references. The source data can be found in the raw data folder and the code folder contains r code made in an rmd file. The raw data is sourced using a computer path, so that may need to be uptaded if downloaded to check the code.



# Midpoint Check In
Part 3. Develop at least 2 possible research questions

Question 1: How do concentrations of different metals (Li, Mn, Co, U) vary across Midwestern watersheds?
  I want to compare different metal concentrations across different watersheds to see if certain land use types affect metal concentration. By comparing land use types, I want to see if the amount of metal changes betwen agricultural land use, urban land use, and undeveloped land. I also want to see if I can compare metal usage 
  A lot of heavy metals are toxic, so understanding how land use changes metal concentration can help identify areas in need of heavier drinking water treatment. Li, Mn, and Co all interest me as specifically metals used in batteries, so understanding these metals specifically could help identify locations to try metal recovery from waste streams. U is interesting as Illinois uses a lot more nuclear power than other states, so I want to compare Illinois uranium concentration to other states.
  I would need to find measures of metal concentration and land use type. Both of these I could probably find on USGS databases, and I'll look into Midwestern state EPA databases as well. 
  To analyze the data, ANOVA would be appropriate as a way to compare land use type to each metal concentration. A regression model could be useful to compare concentration as a function of distance from metropolitan area.

Potential Datasets:
Name: Datasets from Groundwater-Quality and Select Quality-Control Data from the National Water-Quality Assessment Project, January through December 2016, and Previously Unpublished Data from 2013 to 2015
Source: USGS (DOI: 10.5066/P9W4RR74)
Coverage: 648 wells across the U.S., most data during the year 2016 with some data going back as early as 2012.
Main variables: P01035_Cobalt_wf, P01056_Manganese_wf, P01130_Lithium_wf, P22703_Uranium_wf
File format: zip containing .txt files

Name: Annual National Land Cover Database
Source: USGS (DOI: 10.5066/P94UXNTS)
Coverage: Contiguous 48 states, 1985-2024
Main Variables: Land Cover Product
File format: tiff image

Name: Heavy metal
Source:
Link: https://www.kaggle.com/datasets/ziya07/soil-heavy-metal

Link: https://www.ars.usda.gov/research/publications/publication/?seqNo115=410343


Preliminary Method Plan: 
 - match well locations with land cover database using latitude and longitude
 - identify closest urban areas and get distances
 - compare metal concentration with ANOVA

Question 2: How do toxic metal(loid) concentration from fertilizer (As, Cu, Zn, Ni) in water vary across different counties in the midwest? How does this change when accounting for county income? How does this change with high flow events?

  Some metals are common in fertilizers (the metals specified come from article (DOI: 10.1038/s41598-024-79681-9)), which can enter waterways from runoff and potentially enter drinking water. Understanding how the concentration varies with time and precipitation can indicate when water needs significant treatment or when people should primarily use bottled water. Additionally, seeing if this changes with median coutny income could help indicate where state funding should go.
  I would need data on water flow and precipitation, metal concentration, and county median income. 
  USGS could provide some useful data, as well as the U.S. census bureau. I also want to look at midwestern state data to see slightly more detailed measurements.
  I want to perform a  time series analysis on the concentration over time and see how that compares to the time series of changing flow conditions of water. I also want to compare spatially county income with metal concetnration, especially at peak metal concentrations. I think it would be interesting to use ANOVA to compare the impact of income bracket to maximum metal concentration.

Name: Datasets from Groundwater-Quality and Select Quality-Control Data from the National Water-Quality Assessment Project, January through December 2016, and Previously Unpublished Data from 2013 to 2015
Source: USGS (DOI: 10.5066/P9W4RR74)
Coverage: 648 wells across the U.S., most data during the year 2016 with some data going back as early as 2012.
Main variables: P62453_Arsenate_wf, P62452_Arsenite_wf, P01040_Copper_wf, P01090_Zinc_wf, P01065_Nickel_wf
File format: zip containing .txt files

Name: Water Data for the Nation
Source: USGS (https://waterdata.usgs.gov/)
Coverage: Whole U.S.
Main Variables: Water Quality, Precipitation, Streamflow
File format: 

Name: US Census Income Data
Source: US Census Data
Coverage: Whole U.S., (choose 2016)
Main Variables: Median income
