# Visualization of Maize and Sorghum Productivity and Yield in the Karamoja Region of Uganda
## Project Overview 
>[Karamoja](https://en.wikipedia.org/wiki/Karamoja) is the most food-insecure region of Uganda. One of the main reasons is the low productivity level of the crops due to intense droughts as well as pest and disease outbreaks.

>In Karamoja, several NGOs provide technical support as well as farm inputs to the farmers experiencing extremely low yields. However, they lack visibility into the overall state of the region and often need to rely on some very local sources of information to prioritize their activities.

>Dalberg Data Insights (DDI) has been requested to develop a new food security monitoring tool to support the decision-making of one of those NGOs active in Karamoja.
To do so, Dalberg Data Insights developed a methodology to remotely measure the yield of the two main staple crops of the region (i.e. sorghum and maize) based on satellite images. The agri-tech team just ran the model for the 2017 crop season.

## Research Question
As a Data Scientist, the agri-tech team is asking you to develop an interactive visualization tool of the results for this first crop season. This visualization tool that you will develop will be used as a first mockup of the Food Security Monitoring tool that DDI will develop for the NGO.

Based on your experience, the team expects you to come up with a first draft within the coming 3 working days. They give you carte blanche in terms of structure and functionalities but they know that the client wants:

        i.) At least a map in the dashboard
        
        ii.) The possibility of visualizing the results by district or sub-county (two administrative levels used by the NGO)

## Dataset Files 
Dataset Source [Link](https://archive.org/download/data_20190829/DATA.zip)<br>

        1.) Shapefiles
                i.) Boundaries of Uganda Subcounties
                ii.) Boundaries of Uganda Districts
                iii.) Crop Type Map for Sorghum (i.e. position of the Sorghum fields)
                iv.) Crop Type Map for Maize
        
        2.) Tables
                A.) Yield and Population per Subcounty
                        i.) POP: total population for the sub-county
                        ii.) S_Yield_Ha: average yield for sorghum for the sub-county (Kg/Ha)
                        iii.) M_Yield_Ha: average yield for maize for the sub-county (Kg/Ha)
                        iv.) Crop_Area_Ha: total crop area for the sub-county (Ha)
                        v.) S_Area_Ha: total sorghum crop area for the sub-county (Ha)
                        vi.) M_Area_Ha: total maize crop area for the sub-county (Ha)
                        vii.) S_Prod_Tot: total productivity for the sorghum for the sub-county (Kg)
                        viii.) M_Prod_Tot: total productivity for the maize for the sub-county (Kg)       
                B.) Yield and Population per District
                        i.) POP: total population for the district
                        ii.) S_Yield_Ha: average yield for sorghum for the district (Kg/Ha)
                        iii.) M_Yield_Ha: average yield for maize for the district (Kg/Ha)
                        iv.) Crop_Area_Ha: total crop area for the district (Ha)
                        v.) S_Area_Ha: total sorghum crop area for the district (Ha)
                        vi.) M_Area_Ha: total maize crop area for the district (Ha)
                        vii.) S_Prod_Tot: total productivity for the sorghum for the district (Kg)
                        viii.) M_Prod_Tot: total productivity for the maize for the district (Kg)       
## Findings:
1.	From the distribution of total productivity across the sub-counties, we can see that Namalu SubCounty has the highest productivity at 5,596,386 kgs of both maize and sorghum. Kotido sub-county follows closely with 5,541,496 kgs.

![Total Productivity per SubCounty](https://github.com/leogachimu/tableau_visualization/assets/122081776/507195b3-cfcd-4ffd-bb2b-0a444d465037)

2.	From the distribution of total productivity across the districts, I found out that Kotido district has the highest productivity at **18,642,479 kgs**, followed by Nakapiripirit at **14,970,688 kgs**. The least productivity is in Moroto at only **1,029,412 kgs**.

![Map of Productivity per District](https://github.com/leogachimu/tableau_visualization/assets/122081776/ae5b59de-c656-4570-9603-190751187fdc)

![Total Productivity per SubCounty and District](https://github.com/leogachimu/tableau_visualization/assets/122081776/eb511b16-5bfe-4d5e-b109-39e1c13bb401)

3.	The scatter plot of maize yield vs sorghum yield shows that the yield of maize is higher than that of sorghum in almost all the sub-counties. Also, there is a positive correlation between the two yields, which means that as the yield of maize increases, the yield of sorghum also tends to increase.

![Sorghum-Yield vs Maize-Yield in a SubCounty](https://github.com/leogachimu/tableau_visualization/assets/122081776/1db164b1-1e5b-47ed-a581-fcac3ce5031d)

4.	From both the scatter plot and the tree map of maize yield vs sorghum yield, we can also discover the sub-counties where the yield of maize is high but the yield of sorghum is unusually low. These include:
	- Karita (1,287 kgs/Ha (maize) against 193.9 kg/Ha (sorghum))
 	- Lopeei (1,053 kgs/Ha (maize) against 108.2 kgs/Ha (sorghum)) and
  	- Loroo (196 kgs/Ha (maize) against 200.7 kg/Ha (sorghum))<br>
We can also discover a few sub-counties where the yield of sorghum is relatively high but the yield of maize is unusually low. These include:<br>
	- Katikekile at 546 kgs/Ha (maize) against 311 kg/Ha (sorghum) and
 	- Nyakwae at 779 kgs/Ha (maize) against 329.8 kg/Ha (sorghum)

![Sorghum-Yield vs Maize-Yield in a SubCounty (Treemap)](https://github.com/leogachimu/tableau_visualization/assets/122081776/8e690d4f-0e08-4c14-bfd1-5ef97c00ddeb)


5.	From the distribution of total yield (kgs of both maize and sorghum per hectare) across the sub-counties, we can see that some of the most productive sub-counties include:
	- Namalu in Nakapiripirit District (1,886 kgs/Ha)
 	- Alerek in Abim District (1,780 kgs/Ha) and
  	- Sidok in Kaabong District (1,682 kgs/Ha)<br>  
The 3 least productive sub-counties are:<br>
	- Northern Division (374 kgs/Ha)
 	- Tapac (368 kgs/Ha) and
  	- Southern Division (115 kgs/Ha), all in Moroto District.<br>
On average, Nakapiripirit District has the highest yield (1,620 kgs/Ha) while Moroto District has the lowest yield (483 kgs/Ha).

![Distribution of Total Yield per SubCounty](https://github.com/leogachimu/tableau_visualization/assets/122081776/c0116c58-c549-4ebf-b779-60ff3f4f3e0f)

![Distribution of Total Yield per District](https://github.com/leogachimu/tableau_visualization/assets/122081776/98932c95-d08f-4b65-bad0-9df2791b5ce5)


6.	I also sought to discover the sub-counties and districts with the highest potential productivity that is left unexploited. I did this by creating a field for the sum of yield (maize yield plus sorghum yield) multiplied by the crop area not in use. From the respective distributions, we can see that Kotido District has the highest missed potential productivity at **1,529,039 kgs** and within it, the Kotido subcounty has the highest missed potential productivity at **470,948 kgs**. Moroto District has the lowest missed potential productivity of **11,116 kgs**.
   
![Distribution of Potential Productivity Lost per SubCounty](https://github.com/leogachimu/tableau_visualization/assets/122081776/d7f4fbd7-5903-4366-8bb9-964279a55fe3)

![Distribution of Potential Productivity Lost per District](https://github.com/leogachimu/tableau_visualization/assets/122081776/9b3cf867-0821-46c5-9fc1-d6c0c32c60e4)


## Recommendations:
1.	There is a potential to increase the total production of wheat and sorghum by investing in better technologies, farmer education, and other measures in some of the districts and sub-counties where the production is too low. These include Abim and Moroto districts overall, and Northern Division, Tapac and Southern Division sub-counties in Moroto District.
   
2.	The general trend is that the higher the maize yield in a sub-county, the higher the sorghum yield. Therefore, the NGOs in Karamoja should focus more attention on the sub-counties where there is an unusual correlation between maize yield and sorghum yield. If the maize yield is unusually low compared to other sub-counties with comparable sorghum yield, then there is a likelihood that farmers are following the wrong maize farming practices.
Such sub-counties include Katikekile and Nyakwae.<br>
Similarly, where the sorghum yield is unusually low compared to other sub-counties with comparable maize yield, then there is a likelihood that farmers are following the wrong sorghum farming practices. Such sub-counties include Karita, Lopeei, and Loroo.
	
4.	The districts with the highest overall productivity- Kotido and Nakapiripirit- are also the districts with the highest overall lost production potential. They should therefore be given more attention in optimizing the unexploited crop area in the Karamoja region.

## Tableau Public Dashboard
Please see my dashboards here [https://public.tableau.com/app/profile/leonard.gachimu/viz/MaizeandSorghumProductivityinKaramojaUganda/Dashboard2?publish=yes](https://public.tableau.com/app/profile/leonard.gachimu/viz/MaizeandSorghumProductivityinKaramojaUganda/Dashboard2?publish=yes)
