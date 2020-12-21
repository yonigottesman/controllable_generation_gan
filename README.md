# Controllable Generation with Fixed GANs

Conditional GAN architectures such as [cGAN](https://arxiv.org/abs/1411.1784) learn to generate fake images with a specific condition. For example the generator can be forced to generate images of people smiling, with or without glasses or with a specific hair color. But in order to achieve this, the GAN must be trained alongside with the conditional information. What if you are given a fixed trained GAN that was not trained with additional condition information, is it still possible to force the generator to generate images with specific features? according to this paper: [Interpreting the Latent Space of GANs for Semantic Face Editing](https://arxiv.org/abs/1907.10786), YES you can! 
The paper explores how different features are encoded in the latent space and show how by moving around this space you can control the features of a generated fake image.  

The full post is [here](https://yonigottesman.github.io/2020/11/17/wgan-controllable-generation.html/)

Adding a smile to an image:
![](https://github.com/yonigottesman/controllable_generation_gan/blob/main/images/smile_generation.png)

Removing a smile from an image:
![](https://github.com/yonigottesman/controllable_generation_gan/blob/main/images/no_smile_generation.png)

Changing hair color to black:
![](https://github.com/yonigottesman/controllable_generation_gan/blob/main/images/black_hair.png)
