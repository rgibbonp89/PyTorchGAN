# PyTorchGAN

In this repo you'll find my coding of a simple generative adversarial network. I realized a little while ago that I wanted a better understanding of how GANs work, so I decided to write one in PyTorch as well as a brief presentation on how they work.

My plan is to, at some point, do a similar thing for a couple of other GAN variants (DCGAN, CGAN, WGAN, etc.), but that'll have to wait for a little bit. 

To run the code, just call the following in your terminal:

python3 torchGAN.py --number <number that you want to generate> --epochs <the number of epochs> --glr <the generation learning rate> --dlr <the discriminator learning rate>
  
If you don't specify anything for the command line arguments, the code just executes with default settings.
