**Study:** Analysis for Growth and calcification responce of the common collector urchin, _Tripneustes gratilla_, to projected climate change: Effects of Warming and Acidification.

**Authors:** E Sesno, AS Huffmyer, K Bahr, J Lemus

**Corresponding Author:** E Sesno, Sesno@hawaii.edu

**Abstract** 

As climate change leads to alterations in ecosystem and organism functions, the need to explore the breadth of effects is paramount. Increased sea surface temperatures (SST) and ocean acidification (OA) are major contributors leading to alterations in body size and calcification in marine invertebrates, however the full effects are not fully understood. Ecologically important invertebrates, such as sea urchins, calcify in both larval and post-metamorphic life stages, requiring long-term studies that cover changes into adulthood. The goal of this research is to contribute to the understanding of potential climate change impacts on post-metamorphic calcifying marine invertebrates, specifically the common collector urchin native to Hawaiʻi, _Tripneustes gratilla_. In this experiment, individual _T. gratilla_  from juvenile (~16 mm) to adult (~60 mm) were grown under projected environmental conditions of warming (+2C) and increased acidity (-0.3 pH units) and a combination of both. The objectives were to explore the sensitivity of T. gratilla to warming and OA through comparisons of 1) growth (% change from initial to final diameters) and 2) calcification (calculated ratios through Scanning Electron Microscopy (SEM) images of cross-sections) of the urchin spines. Additional proxies of growth (relative spine length calculated proportionally to body size) and calcification (number of dropped spines) were also measured. Results of this research reveal that warmer temperatures increased growth while acidification reduced calcification at the base of spines with no interactive effects of the two factors. Urchins in low pH treatments shed their spines more readily than those in ambient pH, regardless of temperature, indicating that calcification may be hindered in these acidic conditions. These results suggest that while survivorship and growth were normal, the energy required to keep up with calcification, regardless of temperature change, may be inhibitive for the long term.

**Analysis Scripts**

Statisical analyses are conducted in R Markdown (.rmd) and R (.r) files with data contained in Data folder. Figures are outputted into Figures folder.

Urchin_ClimateChange_Plots.Rmd - Result plots of urchin responses

Urchin_ClimateChange_Analysis.Rmd - Analysis of urchin responses

**Data Files**

Urchin_ClimateChange_Data.csv - All corresponding data from duration of the experiment.

Urchin_ClimateChange_Structure.csv - Categorization of SEM cross-section images of spine bases as organized or disorganized. Quantified patterned vs. not patterned to look for trend between treatments. 

Date_CO2Sys.xls - CO2Sys seawater parameters calculations for a given week of water sampling.

**Variables explained**

*Date

*Day - days from -24 to 126. Day -24 is day got urchins, followed by about 2 weeks of acclimation, followed by ramp up period. Day 1 is actual day desired conditions were reached.

*Treatment - 4 categorical - Amb (ambient), T (heated), OA (acidified), T/OA (heated and acidified)

*Header - numbers 1-8 representing which header was feeding the tanks

*TankID - numbers 1-24 indicate which tank and corresponding urchin. Only one urchin per tank.

*Temperature - 2 categorical - heated and ambient

*pH - 2 categorical - acidified and ambient

*Temp - continuous measurement of temperatures within headers and tanks measured weekly with a YSI probe

*pHspec - continuous measurement of pH within headers and tanks measured spectrophotometrically each week.

*Sal - salinity measured weekly using YSI probe

*Diam1 - one of two diameters measured each week on each urchin

*Diam2 - two of two diameters measured each week on each urchin

*DiamMean - the mean of Diam1 and Diam2

*Growth - growth calculated as ((final – initial / initial diameter)x100). Initial diameter is day 1 at which desired conditions were attained (2 weeks after acclimation, followed by 2 weeks of conditions ramping up).

*Height - height of urchins measured at one time point.

*pCO2out - calculate pCO2 from CO2Sys data (see xls files for calculations)

*AlkTotal - Total alkalinity from titrations

*PartOfSpine - indicates the tip or base of spine cross-sections from SEM imaging

*Chosen - categorical label of 'yes' or 'no' to account for dust on SEM image. If dust was present, half of image wihtout dust was analysed. If no dust present, a 'yes' or 'no' label was randomly assigned to choose side for analysis.

*RatioSEM - the ratio of light to dark pixels calculated in imageJ

*SpineLength - length of spines measured in mm tha were plucked from each urchin.

*RatioLength - ratio of length of spine to total test diameter calculated from (spine length/diameter)x100) 

*SpineCount - number of spines counted to be loose on the bottom of the tanks at the end of the experiment.

*SEMPatterened - number of spine SEM images at the base categorized to have a structured or organized pattern of calcification from each treatment

*SEMNone - number of spine SEM images at the base categorized to have a unstructured or disorganized pattern of calcification from each treatment.

*PcntUnorganized - percent of spine bases to have an unorganized appearance from each treatment.

