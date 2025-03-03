---
title: Conditional Rotationally Invariant VAE
---

In this chapter, we introduce the conditional rotational Variational Autoencoder (CrVAE), a model that combines the principles of conditional encoding and rotational decomposition to achieve a more interpretable representation of physical systems. The CrVAE leverages a latent vector for capturing intrinsic variations, a rotation vector to encode orientation, and incorporates conditional information, such as cation type, to account for system-specific variations. This approach enables the disentanglement of latent factors while preserving the physical and chemical distinctiveness of the system components.

:::{figure} #app:CrVAE_widget_1
:name: fig_CrVAE_widget_1
:placeholder: ./figures/fig_CrVAE_widget_1_placeholder.png
(a) The latent manifold generated from the CrVAE demonstrates A site atoms and (b), B site atoms as reconstructed structure across the latent space. (c), (d), and (e) The latent space distribution with KDE highlights clusters, .
:::


The clear separations and clustering in the latent space reflect the incorporation of physical constraints and rotational invariances.ß


:::{figure} #app:CrVAE_widget_2
:name: fig_CrVAE_widget_2
:placeholder: ./figures/fig_CrVAE_widget_2_placeholder.png
latent maps
:::

The analysis reveals that domain walls, with distinct rotational orientations, are strongly influenced by both unit cell rotation and the conditional variable representing cation type. This highlights the CrVAE's ability to incorporate external physical constraints to uncover meaningful relationships within the data.