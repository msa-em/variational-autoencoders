---
title: Methodology
---

In this notebook, we will comparatively explore the use of several classes of variational autoencoders that allow to separate diffeerent known and unknown factors of variation in the data. These are built based on the [pyroVED](https://github.com/ziatdinovmax/pyroVED) library by Maxim Ziatdinov, and allow to (a) incorporate rotational, translational, or both invariances in the data, and (b) condition the VAE on known classes. Overall, we can create 8 possible combinations:

VAE: conventional variational autoencoder (yields latent vector)

rVAE: rotationally invariant VAE (yields latent vector and latent angle)

tVAE: translationally invariant VAE (yields two components of translation vector and latent vector)

trVAE: translationally and rotationally invariant VAE

C-VAE: conditional VAE creates latent spaces conditioned on parameter

C-rVAE: conditional rotationally invariant VAE

C-tVAE: conditional translational invariant VAE

C-trVAE: conditional rotational and translationally invariant VAE.

Note that VAEs will yield latent vectors and (optionally) translation vector and rotation as outputs, and can be configured to use class as input.


