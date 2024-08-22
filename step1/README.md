# Step1 - Load data and libraries

## Loading data

##### Load the data table
#####  from a local directory C:\Projets_En_Cours\AI_MTPL\__BasingHall\25-May-2021\Results
BH_OCC_wStatus <- read.table("C:/Projets_En_Cours/AI_MTPL/__BasingHall/25-May-2021/Results/BH_OCC_wStatus-IDSorted_25-May-2021.csv", header=TRUE, sep=",")

## Loading the necessary libraries

##### Load the FactoMineR library
library(FactoMineR)
##### Install library factoextra 
library(factoextra)
