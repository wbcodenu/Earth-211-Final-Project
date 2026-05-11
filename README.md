# Earth-211-Final-Project
An Earth Science data analysis project


# Midpoint Check In
Part 3. Develop at least 2? 3? possible research questions

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
Main Variables: Land Cover Product (
File format: tiff image


Preliminary Method Plan: 


Question 2: How do toxic metal(loid) concentration from fertilizer (As, Cu, Zn, Ni) in water vary across different counties? How does this change when accounting for county income?
Metals specified come from article (DOI: 10.1038/s41598-024-79681-9)
