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
##### Load theggplot2 graphics library
> <em>library (ggplot2)</em>
##### Load the FactoMineR library
> <em>library(FactoMineR)</em>
##### Install library factoextra 
> <em>library(factoextra)</em>
