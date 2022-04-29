In this exercise, I used ArcGIS Insights to analyze the United States Drug Enforcement Administration’s (DEA) pain pill database that “tracks the path of every single pain pill sold in the United States - by manufacturers and distributors to pharmacies in every town and city.” Specifically, I explored the flow of pain pills in and out of Mingo County, WV, a county with a substantially high rate of pills per person per year. 


<iframe src="https://insights.arcgis.com/#/embed/1a33dd7a3f55460db591e605f684c163" width="100%" height="1190" frameborder="0"></iframe>

First I downloaded the DEA data from the Washington Post website for Mingo, County WV and converted it from a tsv to an excel file, so that I could load it into ArcGIS Insights. After adding the dataset to ArcGIS Insights, I geocoded the addresses of both the distributors and the pharmacies. I found the process of geocoding points to be much simpler than the same workflow in desktop ArcGIS Pro. 

After geocoding the addresses, I simply dragged the distributor and pharmacy address points to a map card, which automatically generated a link map between distributors (reporters) and pharmacies (buyers) inor Mingo County, WV. I then adjusted the weight of the link to reflect the sum of pill dosage units and added a boundary for Mingo County to the map from available ESRI data.

Finally, I used the “Enrich Data” tool to calculate how many people live within five miles of each of the pharmacy locations using 2010 population data from the U.S. Census Bureau. To display this information, I created two tables: the first comparing the pharmacy with the size of the population within 5 miles of the store, and the second comparing the pharmacy with the dosage units. These tables complement each other, showing both the reach of the pharmacy and amount of opioids distributed. 

The resulting map effectively illustrates the flow of pain pills to the pharmacies in Mingo County. It appears that Cardinal Health near Wheeling, WV is the largest distributor of pain pills to the County. I was surprised by how large the supply chain is - pain pills come from as far as Seattle and Vancouver!

Overall, I was excited by how intuitive ArcGIS Insights was to use for this analysis. I often felt like I could anticipate the necessary actions to complete a step, before reading the instructions in the tutorial. I was especially impressed by ArcGIS Insights’ default of creating a link map between two sets of geocoded addresses. I do not know how to create a link map in ArcGIS Pro. The “Enrich Data” function was also super cool - you can easily bring in other publicly available data to provide context and further analysis. I also enjoyed that I was able to use the online version of ArcGIS Insights to complete the same sophisticated analysis that I would only be able to theoretically complete on a desktop version of ArcGIS Pro. However, this exercise illustrated the difficulties that one would encounter when pulling together various publicly available datasets and trying to pair, aggregate, and analyze them geospatially. This is a challenge regardless of what software you decide to use. 

For an comparison of ArcGIS Pro and ArcGIS Insights, please review the slides below.

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vR0mFM5pMymPlJPby1AEjgxX08dC31PAjIv2Ai6b1TuLTcsLxpGYVdYeX-kk5KbKgle5abQdTn1jOyu/embed?start=false&loop=true&delayms=3000" frameborder="0" width="1440" height="839" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>


[Back to the AdvancedGIS homepage](/README.md)
