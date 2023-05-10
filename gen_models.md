## StyleGAN: A Style-Based Generator Architecture for Generative Adversarial Networks
**Tero Karras, Samuli Laine, and Timo Aila**

**CVPR 2019**

This paper introduces a new method to generate images, under the GAN model paradigm. It borrows the idea of style transfer, and considers an image as a collection of "styles", each of which "controls the effects at a particular scale" [video](https://youtu.be/kSLJriaOumA?t=70).

The model architecture is designed to inject latent code at different scales, representing different styles, 

*[TODO]* how the model is trained isn't known to me yet, and implementation details. Here is a good summary on [CSDN](https://blog.csdn.net/weixin_43135178/article/details/116331140) in Chinese.

*[Opinion]* This idea is very interesting and effectively learns a mixture of styles at different scales (4x4, 8x8, etc). We certainly see that human face attributes are decoupled into several groups (or scales). On a high level, the proposed method introduces an unsupervised way to learn attributes/concepts at different scales, by providing the scale information during training, which is very interesting. Building on top of this work, we can try pursue decoupling of attributes/concepts into finer-grained groups, and not necessarily by scale. The trick is to find some information to provide, in order to decouple those attributes/concepts.
