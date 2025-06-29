# Step5 - Evaluate fairness of the selection process of the startup dossiers

### Saving the group (class) vector table for future use
In the present example, the data tables is located in directory: C:\Projets_En_Cours\AI_MTPL__BasingHall\25-May-2021\Results

> <em>write.csv(grp,"grp.csv", sep=",")</em><br>

NOTE -> The group vector grp is exported and then modified for transfer of a few odd companies into of a group 6 for outliers

> grp_modified <- read.table("grp_modified.csv", header=TRUE, sep=",")

