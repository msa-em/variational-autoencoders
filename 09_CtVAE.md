---
title: Conditional Translationally Invariant VAE
---


In this chapter, we introduce the conditional translational Variational Autoencoder (CtVAE), which incorporates translational vectors ($t_x$, $t_y$) and conditional variables, such as cation type, into the latent space. The CtVAE captures positional shifts alongside intrinsic variations, enabling the analysis of system-specific physical properties. This framework provides a structured approach to studying translation-related phenomena while maintaining the distinct physical and chemical characteristics of the components.

:::{figure} #app:CtVAE_manifold_1
:name: CtVAE_manifold_1
:placeholder: ./figures/Ctvae_manifolds_placeholder.png
(a) The latent manifold generated from the CtVAE demonstrates A and B site atoms reconstructed structure across the latent space. (b) The latent space distribution with KDE highlights clusters.
:::

The clear separations and clustering in the latent space reflect the incorporation of physical constraints and rotational invariances.ß


:::{figure} #app:CtVAE_latent_1
:name: CtVAE_latent_1
:placeholder: ./figures/CtVAE_latent_placeholder.png
latent maps
:::

Both $z_1$, $z_2$, and $t_x$, $t_xy$ appear to capture information about the domain structures. However, this raises the question: are we utilizing an excessive number of latent variables to represent the system?
