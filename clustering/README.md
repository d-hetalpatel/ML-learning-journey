🌍 Earthquake Clustering with DBSCAN and KMeans
 Project Overview

This project compares DBSCAN and KMeans clustering algorithms on earthquake location data.
The dataset (2025_09_04_After_Earthquake_Monthly.csv) contains latitude and longitude of earthquake events, and the goal is to identify earthquake hotspots.

Evaluation metrics used:

Silhouette Score (cluster separation)

Davies-Bouldin Index (DBI) (compactness of clusters)

Calinski-Harabasz Index (CHI) (cluster separation vs cohesion)

⚙️ Steps Performed

Data Preparation

Extracted latitude and longitude features.

Standardized values using StandardScaler.

DBSCAN Clustering

Parameters: eps=0.3, min_samples=10.

Evaluated using Silhouette, DBI, and CH Index.

Visualized hotspots with scatter plots.

KMeans Clustering

Optimal number of clusters found via Elbow Method + KneeLocator.

Best k = 5.

Evaluated with same metrics.

Visualized cluster distribution.

 Results
Algorithm	Silhouette Score ↑	DBI ↓	CH Index ↑	Notes
DBSCAN	0.712	1.070	10,407	Good separation, but clusters less compact
KMeans (k=5)	0.723	0.419	21,375	Best overall: compact, well-separated clusters
Interpretation

DBSCAN

Handles noise and irregular cluster shapes well.

Useful if clusters are non-spherical or you expect outliers.

Here, it performed decently but clusters were less compact.

KMeans (k=5)

Produced strong, compact, and well-separated clusters.

Best fit for this dataset since earthquake hotspots are relatively structured.
