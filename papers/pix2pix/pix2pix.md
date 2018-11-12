
# Introduce

<img src='demo.png' width="600px" />
Many problems in image processing, graphics, and vision involve translating an input image into a corresponding output image.
These problems are often treated with application-specific algorithms, even though the setting is always the same: map pixels to pixels.
Conditional adversarial nets are a general-purpose solution that appears to work well on a wide variety of these problems. Here several results of the method, used the same architecture and objective, and simply train on different data.

# Method

<img src='img2.png' width="600px" />
Training a conditional GAN to map edges→photo. The discriminator, D, learns to classify between fake (synthesized by the generator) and real {edge, photo} tuples. The generator, G, learns to fool the discriminator. Unlike an unconditional GAN, both the generator and discriminator observe the input edge map.

## Objective
<img src='lossimg.png' width="800px" />

The objective of a conditional GAN can be expressed as: <img src='cgan.png' width="400px" div align=right />
<br/>
<br/>
To test the importance of conditioning the discriminator:<img src='gan.png' width="400px" div align=right />
<br/>
<br/>
<br/>
Mix the GAN objective with a more traditional loss: <img src='l1.png' width="400px" div align=right />
<br/>
<br/>
Final objective is: <img src='final.png' width="400px" div align=right />

##  Network architectures
**A defining feature of image-to-image translation problems
is that they map a high resolution input grid to a high resolution
output grid.**
