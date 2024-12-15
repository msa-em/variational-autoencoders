---
title: Translationally Invariant VAE
---

In this approach, the latent space is composed of the intrinsic latent variables along with two additional components representing the translation vector ($t_x$, $t_y$). As a result, the dimensionality of the latent space becomes $N+2$, where $N$ corresponds to the number of intrinsic latent variables. This framework allows us to disentangle and analyze both the intrinsic factors of variation and the translational symmetry within the data.



:::{figure} #app:tVAE_widget_1
:name: fig_tVAE_widget_1
:placeholder: ./figures/fig_tVAE_widget_1_placeholder.png
(a) The latent manifold generated from the VAE demonstrates the reconstructed structure across the latent space. (b), (c), (d), (d), and (f) The latent space distribution with KDE highlights clusters, .
:::

We observe well-defined clusters, which strongly suggest the presence of underlying physical principles governing the system.


:::{figure} #app:tVAE_widget_2
:name: fig_tVAE_widget_2
:placeholder: ./figures/fig_tVAE_widget_2_placeholder.png
latent maps.
:::

The latent maps reveal fascinating insights. The translation vectors closely resemble the polarization components, aligning with the underlying physics of ferroelectrics, where the polarization arises from the shift of the central atom relative to the corner atoms. Simultaneously, the intrinsic latent variables $z_1$, and $z_2$ exhibit chemical contrast and mistilt effects, with minor leakage of polarization information into their representation.