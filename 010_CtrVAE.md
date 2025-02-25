---
title: Conditional Rotationally and Translationally Invariant VAE
---


The conditional translational Variational Autoencoder (CtrVAE) combines translational invariances, conditional encoding, and latent space decomposition to provide a comprehensive representation of physical systems. By leveraging latent vectors for intrinsic variations, translation vectors for positional shifts, and conditional information such as cation type, the CtrVAE effectively disentangles system-specific factors while maintaining the distinct physical and chemical features of the data.

:::{figure} #app:CtrVAE_manifold_1
:name: CtrVAE_manifold_1
:placeholder: ./figures/Ctrvae_manifolds_placeholder.png
(a) The latent manifold generated from the CrVAE demonstrates A and B site atoms reconstructed structure across the latent space. (b) The latent space distribution with KDE highlights clusters.
:::


The distinct separations and well-defined clusters across all combinations of latent variables highlight the effective integration of physical constraints and invariances, ensuring a meaningful representation of the system.


:::{figure} #app:CtrVAE_latent_1
:name: CtrVAE_latent_1
:placeholder: ./figures/Ctrvae_latent_placeholder.png
latent maps
:::

The analysis suggests a potential redundancy in the latent space, as the information encoded in $z_2$ appears to overlap significantly with the angular variable. This overlap indicates that the latent representation may contain more variables than necessary to effectively describe the system, highlighting the need for further optimization or dimensionality reduction to enhance interpretability and efficiency.