KmeansClustering
================

This is week 7 assignment of [Coursera Machine Learning] (http://www.coursera.org/course/ml) class.

Summary
------
In the first part of this program, the K-means clustering algorithm is implemented and applied to compress an image. In the second part, principal component analysis is performed to obtain a low-dimensional representation of face images.

#### K-means Clustering

K-means clustering is an unsupervised learning algorithm that automatically clusters similar data examples together. After random initialization, two step were repeatedly carried out: (i) Assigning each training example x to its closest centroid, and (ii) Recomputing the mean of each centroid using the points assigned to it. To minimize the distortion, multiple random initializations is implemented. Regular 24-bit representation of color image is compressed by reducing the number of colors to 16 colors that best clusters the pixels in three-dimensional RGB space.


Completed methods are summarized below:

 findClosestCentroids.m - Find closest centroids (used in K-means) <br\ >
 computeCentroids.m - Compute centroid means (used in K-means) <br\ >
 kMeansInitCentroids.m - Initialization for K-means centroids <br\ >

Starter codes are listed below:
> ex7.m - Octave/Matlab script for the first exercise on K-means <br\ >
> ex7data2.mat - Example Dataset for K-means <br\ >
> drawLine.m - Draws a line over an exsiting figure <br\ >
> plotDataPoints.m - Initialization for K-means centroids <br\ >
> plotProgresskMeans.m - Plots each step of K-means as it proceeds <br\ >
> runkMeans.m - Runs the K-means algorithm <br\ >

#### Principle component analysis

principal component analysis (PCA) is performed for dimensionality reduction on a 5000 face image dataset. After computing the covariance matrix, SVD is used to compute the principal components. The principle components then can be used to reduce the feature dimension of dataset by projecting each example onto a lower dimensional space.

Completed methods are summarized below:
 pca.m - Perform principal component analysis <br\ >
 projectData.m - Projects a data set into a lower dimensional space <br\ >
 recoverData.m - Recovers the original data from the projection <br\ >
 
 Starter codes are listed below:
 > ex7 pca.m - Octave/Matlab script for the second exercise on PCA <br\ >
 > ex7data1.mat - Example Dataset for PCA <br\ >
 > ex7faces.mat - Faces Dataset <br\ >
 > bird small.png - Example Image <br\ >
 > displayData.m - Displays 2D data stored in a matrix <br\ >
