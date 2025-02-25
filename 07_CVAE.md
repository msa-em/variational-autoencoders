---
title: Conditional VAE
---



However, the previous analysis presented a significant limitation: it assumed a shared latent representation for both A-site and B-site cations, despite their inherently distinct physical and chemical roles. To address this issue, we now employ a conditional Variational Autoencoder (cVAE), where the cation type is incorporated as a known variable. By conditioning the latent space on this additional information, we aim to achieve a more accurate and physically meaningful representation of the system. 

Condition 1: Set the conditiona as A and B site atoms of the material

:::{figure} #app:CVAE_manifold_1
:name: CVAE_manifold_1
:placeholder: ./figures/CVAE_manifolds_placeholder.png
(a) The latent manifold generated from the CVAE demonstrates A and B site atoms reconstructed structure across the latent space. (b) The latent space distribution with KDE highlights clusters.
:::

The two latent spaces shown are for A-type cations and B-type cations, modeled separately using the Conditional Variational Autoencoder (C-VAE). This approach allows us to study each cation type individually and see how they behave in the latent space.

Manifold for A-type cations:

1. This pattern suggests that the variations in the A-type cations are smooth and follow an organized structure, similar to their positions in the crystal lattice.

Manifold for B-type cations:

2. This pattern looks slightly different from the A-type manifold.
The differences might come from physical changes in the B-type cations, like polarization shifts or small distortions in their positions.


:::{figure} #app:CVAE_latent_1
:name: CVAE_latent_1
:placeholder: ./figures/CVAE_latent_placeholder.png
latent maps
:::

We observe intriguing new behavior, particularly anomalous variations in $z_1$ at the "diffuse" domain walls. This raises questions about the underlying mechanisms. To further investigate, we propose introducing invariances into the analysis to gain deeper insights.