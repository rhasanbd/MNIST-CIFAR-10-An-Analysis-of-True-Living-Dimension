# MNIST & CIFAR-10 - An Analysis of True Living Dimension

In this notebook, we analyze the dimension of the images of two popular Machine Learning (ML) image datasets: MNIST handwritten digits & CIFAR-10. Our goal is to understand the **true living space of these two high-dimensional datasets**. 


## MNIST
The MNIST (Modified National Institute of Standards and Technology) dataset contains 70,000 small images of digits handwritten by high school students and employees of the US Census Bureau. Each image is labeled with the digit it represents.

Each image is **grayscale** 28 x 28 pixels, and each feature simply represents one pixel’s intensity, from 0 (white) to 255 (black).

## CIFAR-10
The CIFAR-10 (Canadian Institute For Advanced Research) dataset contains 60,000 images of 10 different classes: airplanes, cars, birds, cats, deer, dogs, frogs, horses, ships, and trucks.

Each image is **RGB (color)** with 32 x 32 x 3 pixels.


- While the images of the MNIST dataset are "normalized" (centered and similar background), the images of the CIFAR-10 dataset has a lot of variations.


## Tasks

For this analysis, we perform two tasks.

- Task 1: Compare Grayscale and RGB Images via Pixel-level Visualization

- Task 2: True Living Space Analysis: MNIST & CIFAR-10 


## Summary of Observations



We will see that although the MNIST image dimension is 784 (28 x 28), only a small fraction of the pixels are non-zero. A large majority of the pixel locations, which constitute the background, are zeros. All images share the same background.

- Therefore, the true living space of MNIST images is low-dimensional.



On the other hand, in CIFAR-10 imges all pixel locations have non-zero values. By analyzing the background of the CIFAR-10 images, we find that the background of the images vary. It indicates that the images occupy the entire pixel space, i.e., images are 3072-dimensional (32 x 32 x 3).

- Therefore, the true living space of CIFAR-10 images is high-dimensional.
