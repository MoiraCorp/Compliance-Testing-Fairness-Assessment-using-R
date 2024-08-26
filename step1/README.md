# Step1 - Load data and libraries

## Loading data into R

The data table BH_OCC_wStatus-IDSorted_25-May-2021.csv may be downloaded from this Github sub-directory (/step1)<br>
either individually or through a Github site cloning process

##### Load the data table from your local Windows directory into R
In the present example, the data table is located in directory: C:\Projets_En_Cours\AI_MTPL\__BasingHall\25-May-2021\Results
> <em>BH_OCC_wStatus <- read.table("C:/Projets_En_Cours/AI_MTPL/__BasingHall/25-May-2021/Results/BH_OCC_wStatus-IDSorted_25-May-2021.csv", header=TRUE, sep=",")</em><br>

<strong>IMPORTANT Note:</strong> The file paths in R follow the Linux standard<br> so that the "\\" character used in Windows file paths
need to be changed to character "/"

## Loading the necessary libraries

This training exercise uses several specialized R libraries: 
<ul>
<li><strong>ggplot2</strong><br>
on CRAN: ggplot2: Create Elegant Data Visualisations Using the Grammar of Graphics (https://cran.r-project.org/web/packages/ggplot2/index.html)<br>
see also: ggplot2 R Documentation (https://www.rdocumentation.org/packages/ggplot2/versions/3.5.0)<br>
with examples in: Data visualization (https://r4ds.hadley.nz/data-visualize) 
</li>
  <li><strong>plotly</strong><br>
on CRAN: plotly: Create Interactive Web Graphics via 'plotly.js (https://cran.r-project.org/web/packages/plotly/index.html)<br>
see also: Interactive web-based data visualization with R, plotly, and shiny (https://plotly-r.com/)<br>
</li>
<li><strong>FactoMineR</strong><br>
on CRAN: FactoMineR: Multivariate Exploratory Data Analysis and Data Mining (https://cran.r-project.org/web/packages/FactoMineR/index.html)<br>
</li>
<li><strong>factoextra</strong><br>
on CRAN: factoextra: Extract and Visualize the Results of Multivariate Data Analyses (https://cran.r-project.org/web/packages/factoextra/index.html)<br>
</li>
</ul>
<strong>IMPORTANT Note:</strong> Before using the "library" function in R, one needs to check that the correponding packages have been loaded from CRAN<br>
<em>Check R or RStudio documentation on how to install CRAN packages</em> 

##### Load theggplot2 graphics library
> <em>library (ggplot2)</em>
##### Load plotly graphics library
> <em>library(plotly)</em>
##### Load the FactoMineR library
> <em>library(FactoMineR)</em>
##### Install library factoextra 
> <em>library(factoextra)</em>
