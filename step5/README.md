# Step5 - Evaluate fairness of the selection process of the startup dossiers

### Saving the group (class) vector table for future use
In the present example, the data tables is located in directory: C:\Projets_En_Cours\AI_MTPL__BasingHall\25-May-2021\Results

> <em>write.csv(grp,"grp.csv", sep=",")</em><br>

NOTE -> The group vector grp is exported and then modified for transfer of a few odd companies into of a group 6 for outliers

> <em>grp_modified <- read.table("grp_modified.csv", header=TRUE, sep=",")</em>

> <em>\# Composite plot of ellipses with status</em><br>
> <em>grp <- as.factor(grp_modified$GrwithStat)</em><br>
> <em>\# Here we want to have the ellipses of Status=Dismissed in grey</em><br>
> <em>\# See deriving color palette for 9 classes : http://www.sthda.com/english/wiki/colors-in-r</em><br>
> <em>fviz_pca_biplot(occ.pca, axes = c(2, 3),</em><br> 
> <em>		habillage = grp,</em><br>
> <em>		palette = c("#FF0099", "#993FFF", "#0066CC", "#33CCCC", "#009966", "#AAAAAA","#AAAAAA", "#AAAAAA", "#AAAAAA", "#AAAAAA", "#AAAAAA", "#AAAAAA"),</em><br>
> <em>             	addEllipses = TRUE)</em><br>

<img src="Biplot_Modified+Ellipse_bh_occ.pca.23_K-means_5 groups+Status.png" alt="drawing" width="70%"/>

> <em>\# Statitics for each group of companies</em><br>
> <em>grp_stat <- describeBy(OCC_wStatus[,c(4:14,15:17)],grp_modified$Group, mat=TRUE)</em><br>



