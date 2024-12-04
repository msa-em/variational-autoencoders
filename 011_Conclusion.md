---
title: Conclusion
---



Troughout htis notebook, we have taken you on the whirlwind tour of the invariant and conditional VAEs. By intorducing the invariances, we both allow the data to speak for itself (via latent variables), and separate physical meaning (translations and rotations). We have also tried to explain the logic that we can follow in choosing the right VAE, going forward and backward between the data and physical interpetations and expectations. ALready in this form, you can use thi snotebook for your own data sets - whether these are ferroics, multiphase materials, or otehr systems.

However, you can also ask questions:

How do we know that the number of latents and chosen invariances are correct?
How do we know which descriptor to choose (here we use the patch of size w, and w can be a variable. Also, we can choos emore complex descriptors, e.g. rectangular pathches w1,w2, or even more complex objects)
What about more complex invariances?
After all, here we eseentially did iterative epxloration in small, but still combinatorial space. It turns out, we can optimize thes eparameters using the reward function based approach - stand by for futher papers form our group!

