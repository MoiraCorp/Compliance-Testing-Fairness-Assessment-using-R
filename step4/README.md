# Step4 - Display clusters statistics of retained clusters

## Determine the k=5 clusters PCA factor space 2-3

Note: We are reusing the df table which was built before from the extracted PCA 2-3 factor scoresfactor
### Pre-determine the pseudo-random series used to determine the initial k-means centers
Note: This determination is done so that clusters will be stable between R runs
> <em>set.seed(123)</em>
### Compute k-means with k = 5
> <em>km.res <- kmeans(df, 5, nstart = 25)</em>

## Display results as "coverage" polygons

### Plotting the cluster results in axes 1,2 plane (Here, the entire data space as its dimensions are 2)
NOTE: 
 - Here we have "axes = c(1,2)" because by construction we have only 2 components (i.d., factor scores)
 - The "palette" parameters for 9 potential clusters are preset following : Colors in R (http://www.sthda.com/english/wiki/colors-in-r)
> <em>fviz_cluster(km.res, data = df,<br>
             palette = c("#00AFBB","#2E9FDF", "#E7B800", "#FC4E07", "#3399FF", "#FF3399", "#336600", "#330033", "#009966"),<br>
	     axes = c(1,2), repel = TRUE,<br>
             ggtheme = theme_minimal(),<br>
             main = "Partitioning Clustering Plot"<br>
             )   + scale_x_reverse()<br>
</em>

<img src="BHP-25-May-2021_PCA-Biplot_2-3_Kmeans.png" alt="drawing" width="70%"/>
<stong>-> INTERPRETATION - The separability of the 5 determined groups is rather good</strong>

## Display cluster results in the original original factor space 2-3 biplot
