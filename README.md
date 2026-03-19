# ENV_710_Final_Project
# Water Quality of Streams in Durham, NC

## Background Information
The City of Durham sits on top of a major drainage ridge, which creates a unique hydrological divide that splits the streams between two of North Carolina’s largest river basins: the Neuse River Basin (North), where streams like the Eno River flow into Falls Lake, eventually reaching the Pamlico Sound, and the Cape Fear River Basin (South), where streams like New Hope Creek flow into Jordan Lake (Harden et al., 2024; Stow and Borsuk, 2003). This feature makes the city a critical waterhead city, where urban activities heavily affect the regional freshwater resources. The two major lakes that Durham’s streams flow into serve thousands of households in Raleigh, Cary, Pittsboro, and other municipalities in Central North Carolina.

In July 2025, Tropical Storm Chantal incurred significant, unprecedented damage in Durham. Over 150 residents were displaced in Orange County, and initial damage costs were estimated at more than $50 million (Grubb, 2025; Medina and Albeck-Ripka, 2025). However, data gaps have hindered swift action in response to the storm, and how the extreme weather event affects the local water quality is unclear. Therefore, our goal is to investigate water quality parameters and answer the research questions:
How do Durham’s Northern and Southern watersheds differ in freshwater quality?
How does water quality change in Durham before and after extreme weather events, such as Tropical Storm Chantal?

## Relevance and Significance
Tropical storms increase nutrient pollution in North Carolina’s water systems. Runoff from tropical storms may double nitrogen and triple phosphorus loads in watersheds, which degrades aquatic habitats (Paerl et al., 2018). Nutrient pollution results in algal blooms that limit dissolved oxygen and lead to fish kills. These pollutants may also negatively affect human health if ingested in sufficient quantities (Manuel, 2014). Most importantly, tropical storm impacts are not experienced uniformly. Minority and lower socioeconomic populations suffer disproportionately from poor water quality (Levin, 2024). Our analysis of water quality post-Chantal will inform planning efforts to mitigate future storm events and identify target areas for policy interventions (Pederson, 2025).

## Data Description
Our study utilizes a public water quality dataset compiled by Durham’s municipal Environmental and Street Services (City of Durham, 2026). This dataset consists of water quality measurements conducted by the city at various sampling locations, and covers all the major streams within the city boundary as the sampling unit. The data entries include chemical (e.g., organic and metal contents), physical (e.g., temperature, turbidity), and temporal attributes. Among all the variables, we chose Dissolved Oxygen (DO) as the primary dependent variable, as it is the output of a stream’s ecological health and shows the actual capacity of the water to support life. In North Carolina, the state-wide standard requires Class C waters to have a daily average of at least 5.0 mg/L DO to protect aquatic life (NC DEQ, 2026). Meanwhile, for the independent variables, we choose from a combination of both continuous (e.g., total nitrogen, total phosphorus, organic carbon, total suspended solids, etc.) and categorical variables (e.g., sub-watershed, temporal phases).

## Data Limitations
We recognize that this dataset has limitations in the following areas:
Temporal alignment: Though the city samples all the streams on a monthly basis, the measurements are not always conducted on a fixed date. Hence, generalizing into year/month for temporal alignment may create potential averaging error. A storm event can cause large changes within 24 hours, while monthly samplings might not capture that spike.
Detection limits: Water quality sensors have their lowest detection limits, and when the limits are reached, the data will be reported as an estimation, which could skew the true data distribution. Also, for heavy metal occurrences, reporting the data as continuous variables might be less informative compared with binary variables (present/absent).
Spatial Autocorrelation: Sampling sites located on the same river are not independent, and therefore, we have to be careful when comparing different sites and conducting regression analyses that assume independent observations.

## References
Durham, the City of. (2026). Water Quality Data Web Portal. Retrieved February 18, 2026. http://www.durhamwaterquality.org/ 
Grubb, Tammy. “Chantal Floods Cause $56m in Damages to Orange County Buildings and Businesses.” The News & Observer, July 16, 2025. https://www.newsobserver.com/news/local/counties/orange-county/article310619555.html. 
Harden, S., Journey, C., and Etheridge, A. (2024). Assessment of Nutrient Load Estimation Approaches for Small Urban Streams in Durham, North Carolina. US Geological Survey, Scientific Investigations Report 2024-5053. https://doi.org/10.3133/sir20245053 
Levin, R., Villanueva, C. M., Beene, D., Cradock, A. L., Donat-Vargas, C., Lewis, J., Martinez-Morata, I., Minovi, D., Nigra, A. E., Olson, E. D., Schaider, L. A., Ward, M. H., & Deziel, N. C. (2023). US drinking water quality: Exposure risk profiles for seven legacy and emerging contaminants. Journal of Exposure Science and Environmental Epidemiology, 34(1), 3–22. https://doi.org/10.1038/s41370-023-00597-z
Manuel, J. (2014). Nutrient pollution: A persistent threat to waterways. Environmental Health Perspectives, 122(11). https://doi.org/10.1289/ehp.122-a304
Medina, E. and Albeck-Ripka, L. (July 7, 2025). Severe Flooding in North Carolina After Chantal Dumps Heavy Rain. New York Times. https://www.nytimes.com/2025/07/07/weather/tropical-storm-chantal-floods-north-carolina.html
North Carolina Department of Environmental Quality (NC DEQ). (2026). Surface Water Standards. Accessed February 20, 2026. https://www.deq.nc.gov/about/divisions/water-resources/water-planning/classification-standards/surface-water-standards 
Paerl, H.W., Crosswell, J.R., Van Dam, B. et al. (2018). Two decades of tropical cyclone impacts on North Carolina’s estuarine carbon, nutrient and phytoplankton dynamics: implications for biogeochemical cycling and water quality in a stormier world. Biogeochemistry 141, 307–332. https://doi.org/10.1007/s10533-018-0438-x
Pederson, M. (2025, November 18). NASA-Funded Tool Tracks Floods and Water Risks in North 
Carolina. NASA. https://www.earthdata.nasa.gov/learn/data-in-action/nasa-funded-tool-tracks-floods-water-risks-north-carolina 

Stow, C. and Borsuk, M. (2003). Assessing TMDL Effectiveness Using Flow-Adjusted Concentrations:  A Case Study of the Neuse River, North Carolina. Environmental Science and Technology, 37(10).
https://doi.org/10.1021/es020802p 

