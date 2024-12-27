---
title: Clustering
---

We’re applying clustering to the descriptors extracted from subimages to group similar structural features and then visualizing the clusters to better understand the patterns in the data.

Clustering with Gaussian Mixture Model (GMM)

1. GMM on Raw Descriptors (Fit_GMM):

    The function Fit_GMM is applied directly to the descriptors, with 5 clusters specified and a “full” covariance type. This model assumes the data can be represented by a mixture of 5 Gaussian distributions with unrestricted covariance matrices (i.e., allowing each cluster to have its unique shape).

Outputs: Cluster labels assigned to each subimage, indicating the group each subimage belongs to.

valid_subimages: The subset of descriptors that were successfully clustered.

2. PCA and GMM Combined (Fit_PCA_GMM):

    The Fit_PCA_GMM function applies Principal Component Analysis (PCA) to reduce the dimensionality of the descriptors from high-dimensional space down to 2 principal components (PCs).


:::{figure} #app:gmm_widget_1
:name: fig_gmm_widget_1
:placeholder: ./figures/fig_gmm_widget_1_placeholder.png
clusters.
:::

As you can see, the use of the GMM clustering in the original descriptor space (i.e. 1600 dimensional space if the descriptor is 40x40 image patch) gives a pretty good separation of several domain configurations and substrate. The GMM clustering of the data set that was dimensionality reduced by PCA shows additional details - for example, you can see that the domain on the bottom is now split in two parts. Practically, it happens because the STEM imaging is not ideal, and the image suffers from mis-tilt effect (small deviation of the column direction from the beam direction). Npte that this mistilt effect is not visible on the polarization field maps. So we can start asking questions like:

1. What is the “right” way to analyze the data?
2. What other information on materials properties is hidden in the images?
3. And how can we extract it combining both the data-driven and physical insights?
Let’s explore this using the VAE approaches!



