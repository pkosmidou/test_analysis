# mtcars_clustering_

Creating by Nena Kosmidou
## Written code for creating a Cluster Dendogram

dat=mtcars
pmatrix=scale(dat)
d=dist(pmatrix)
c=hclust(d,method="ward.D2")
plot(c)
rect.hclust(c,k=4)
