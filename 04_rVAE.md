---
title: Rotationally Invariant VAE
---

Unlike a standard VAE, the rVAE decomposes the latent representation into two components: a latent vector and a rotation vector. While the latent variables aim to encode the intrinsic factors of variation within the data, the rotation vector captures a physically interpretable property – the orientation of the descriptors.

When implementing the rVAE with a 2D latent space, the system effectively utilizes three latent variables: two variables for the regular latent space and one additional variable to encode the rotational orientation. This decomposition introduces a clear physical meaning to part of the latent representation, specifically the rotational degree of freedom, bridging the gap between the statistical encoding and the underlying physics of the system.



:::{figure} #app:rVAE_widget_1
:name: fig_rVAE_widget_1
:placeholder: ./figures/rVAE_manifold_placeholder.png
(a) The latent manifold generated from the VAE demonstrates the reconstructed structure across the latent space. (b), (c), and (d) The latent space distribution with KDE highlights clusters, .
:::

The clusters in latent space become more separated. These clearly correspond to the A- and B type cations now.


:::{figure} #app:rVAE_widget_2
:name: fig_rVAE_widget_2
:placeholder: ./figures/rVAE_latent_placeholder.png
Latent_maps.
:::

We now observe promising and insightful results: the domain walls are clearly associated with the rotation of the unit cells. Notably, the analysis reveals both positive and negative domain walls, highlighting distinct rotational orientations across the structure. This outcome demonstrates the capability of the rotationally invariant VAE to uncover physically meaningful relationships within the data. 