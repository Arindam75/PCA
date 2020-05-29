# Principal Component Analysis and Clustering

In this problem we look at real world problem of clustering 168 coutries based on some Macro-economic indicators. Some examples are
child moratlity, exports and imports expressed as percentage of GDP etc. The dataset consists of nine such features
for all the 168 countries. Our objective is to explore, if the countries fall into distinct clusters based on some similarities. This could
help us identify countries desperate in need of financial need.

We start by asking by removing Outliers. These are countries with very high GDP per capita. Then we implement Principal Component Analysis ( PCA )
for dimensionality reduction. We notice that , even with 6 features we are able to retain 98% of the variance in the data.

### K-Means Cluster

With the number of features reduced to six, we implement K-Means cluster on the dataset. The initial choice of K is done by __Elbow Method and Solhouette Score__.
In both cases, we notice that K=4 is optimum. Since with six dimensions, we cannot visualize the data, so we choose to take pairs of features
like Life Expectency vs Child Mortality, Health Spending vs Child Mortality, income vs child mortality.

We notice our itutions coming true in the visualizations. Countries doing ver poorly in terms of child mortality are poor in these three metrics as well.

### Hierarchical Clsutering

In this section we try three methods, __Ward, Single and Complete__. It turns out, that the Ward method gives us the cleanest clusters.

### Conclusions

We notice that both methods give us almost the same countries which need financial-aid. The countries doing poorly in terms of child mortality
are have very poor macro-economic indicators.


