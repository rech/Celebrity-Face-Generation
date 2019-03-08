# Celebrity Face Generation
Building a **Deep Learning** model which generates realistic faces of the celebrities who doesn't even exist.
\
\
\
!["Generated celebrity faces"](/face_generation_image.png "Generated celebrity faces")



# Overview
The model uses DCGAN to generate random faces which looks realistic.

* ### Discriminator :
  1) Convolutional Layer 3 -> 32
  2) Convolutional Layer 32 -> 64
  3) Convolutional Layer 64 -> 128
  4) Convolutional Layer 128 -> 256
  5) Flatten
  6) Fully connected Layer 1024 -> 1

* ### Generator :
  1) Fully connected Layer 100 -> 1024
  2) Unflatten
  3) Deconvolutional Layer 256 -> 128
  4) Deconvolutional Layer 128 -> 64
  5) Deconvolutional Layer 64 -> 32
  6) Deconvolutional Layer 32 -> 3


# Dependencies
* Python
* PyTorch
* Numpy
* Matplotlib


# Steps involved
1. Load and preprocessing the data 
2. Define Discriminator and Generator
3. Building the model
4. Training and validating loss
5. Generating faces
