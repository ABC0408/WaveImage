## Structure
## Coarse-to-fine generator
- train a residual network G1 on lower resolution images
- another residual network G2 is appended to G1 and the two networks are trained jointly on high resolution images
## Multi-scale discriminators
- High-resolution images are not only difficult to generate, but also difficult for computers to identify true and false.
-  To identify whether a high-resolution image is real or synthetic, you need a discriminator that is very receptive, that is,
  either a deep network or a large convolution kernel. Both of these methods increase network capacity, resulting in easy 
  overfitting and more memory during training.
- They propose using multi-scale discriminators that have an identical network structure but operate at different image scales.
  1. Downsample the real and synthesized highresolutionimages by a factor of 2 and 4 to create an image pyramid of 3 scales 
    as D1, D2 and D3.
  2. The discriminators D1, D2 and D3 are then trained to differentiate real and synthesized images at the 3 different scales, 
    respectively.
  3. The discriminator that operates at the coarsest scale has the largest receptive field. It has a more global view of the image and 
    can guide the generator to generate globally consistent images.
  4. The discriminator at the finest scale encourages the generator to produce finer details. 
## Improved adversarial loss
### Condition-GAN loss
### Feature matching loss
  Incorporating a feature matching loss based on the discriminator: extract features from multiple layers of the discriminator
  and learn to match these intermediate representations from the real and the synthesized image.
