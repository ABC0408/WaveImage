in the wave-image.ipynb file, It provides a way to build a bridge between pictures and voice.
# Plan
After convert audio to wave-image, now my task also change to image to image translation.
- Part1： read some papers about image-to-image translation
- Part2： thinking about the difference between wave-image and others real world image

# Part 1:
## Papers
1. - [x] **Pix2Pix** Image-to-Image Translation with Conditional Adversarial Networks [[paper](https://arxiv.org/pdf/1611.07004.pdf)] [[code](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)] [[notes](./papers/pix2pix/pix2pix.md)]
2. - [x] **Pix2PixHD** High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs [[paper](https://arxiv.org/pdf/1711.11585.pdf)] [[code](https://github.com/NVIDIA/pix2pixHD)] [[notes](./papers/pix2pixhd/pix2pixhd.md)]
3. - [ ] **CycleGAN** Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks [[paper](https://arxiv.org/pdf/1703.10593.pdf)] [[code](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)] [notes]
4. - [ ] **BicycleGAN** Toward Multimodal Image-to-Image Translation [[paper](https://arxiv.org/pdf/1711.11586.pdf)] [[code](https://github.com/junyanz/BicycleGAN)] [notes]



# Part 2:
1. the object in the image has their own shape, color ,,,. In the wave-image, it consists of different words. Each word has their own shape, color. 
