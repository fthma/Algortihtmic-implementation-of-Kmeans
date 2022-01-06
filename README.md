# Algortihtmic-implementation-of-Kmeans
The following project implements the  unsupervised Learning algorithm called K-Means algorithm

Introduction:
The following project implements an unsupervised Learning algorithm called K-Means. K-Means is a clustering algorithm which has applications like detecting groups of similar visitors to a site, visualization, anomaly detection etc. In the K-means algorithm the k depicts the number of clusters we wish to divide into. At first based on the k value, a k number of centroids is initialized to any random values either from within or outside the given dataset X. Each point is taken and the  Euclidean distance between it and  the centroids is found and the point is put into the cluster of the centroid that it is closest to. After the clusters are formed new centroids are calculated by taking the mean of the points in each cluster and the process reiterates  again with the new centroids. This process keeps iterating unless all the points are put into the same cluster again or the new centroids calculated remain unchanged or simply iterates a specified number of times. The clusters formed in the last iteration are the result. 
Although K-means algorithm is an unsupervised algorithm it requires us to have a pre-knowledge about picking the right k value.

My program makes use of the functions in openCv, NumPy libraries of python for processing the image in order to implement the K-means algorithm. The colour image is first read by making use of the cv2.imread(). 
In order to find the strongest corners in the image, cv2.goodFeaturesToTrack() is used. These corners are displayed on the image as small dots by using the cv2.circle() function.
