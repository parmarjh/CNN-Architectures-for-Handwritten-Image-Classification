# CNN Architectures on MNIST: Custom, LeNet & VGGNet-inspired #

To classify images containing handwritten digits using multiple custom-built CNN architectures, which may or may not are inspired from standard Convnet architectures such as LeNet, AlexNet, VGGNet, ResNet etc. A comparison between performance of different architectures are done.

## Purpose ##

The purpose of this study is to **try 3 drastically different Convnet Architectures on MNIST image database**. The implementation is done in Keras.

## Steps at a Glance: ##

1. Take the famous MNIST dataset as input. http://yann.lecun.com/exdb/mnist/

2. Feed it into **3-layered Convnet Architecture design inspired by LeNet, 1998 paper by LeCunn**.

3. Find the **accuracy and draw the Loss vs Epoch Plot**.

4. Introduce Batch Normalization and Dropouts.

5. Evaluate the model again by estimating accuracy and drawing loss diagram.

6. Feed same input to **5 layered Convnet Architecture design inspired by VGGNet, 2014 paper by Andrew Zisserman**.

7. Introduce Pooling, Dropouts & evaluate the model again.

8. Feed same input to **7 layered Convnet Architecture self-designed with different-sized filters & dense layers**.

9. Introduce Batch Normalization and Dropouts & evaluate the model again.

10. Analyze the output from the above 3 architectures and draw conclusions.

## Model 1: LeNet Inspired 3-Convolution Layer Architecture ##

<p align="center">
    <img src="https://github.com/AdroitAnandAI/CNN-Architectures-for-Handwritten-Image-Classification/blob/master/images/1.5.1.PNG">
</p>

<p align="center">
    <img src="https://github.com/AdroitAnandAI/CNN-Architectures-for-Handwritten-Image-Classification/blob/master/images/1.5.2.PNG">
</p>

## Model 2: VGGNet Inspired 5-Convolution Layered Architecture ##

<p align="center">
    <img src="https://github.com/AdroitAnandAI/CNN-Architectures-for-Handwritten-Image-Classification/blob/master/images/1.6.1.PNG">
</p>

<p align="center">
    <img src="https://github.com/AdroitAnandAI/CNN-Architectures-for-Handwritten-Image-Classification/blob/master/images/1.6.2.PNG">
</p>

## Model 3: 7-Layered CNN Architecture ##

<p align="center">
    <img src="https://github.com/AdroitAnandAI/CNN-Architectures-for-Handwritten-Image-Classification/blob/master/images/1.7.1.PNG">
</p>

<p align="center">
    <img src="https://github.com/AdroitAnandAI/CNN-Architectures-for-Handwritten-Image-Classification/blob/master/images/1.7.2.PNG">
</p>

## Conclusions ##

1. The **performance of standard-model inspired networks are found higher** than complex custom built architectures.

2. The **convergence of model M2 happened much before Model 1. Number of epochs required is less**.

3. The **99.5% accuracy of VGGNet-inspired M2 model is better than LeNet-inspired M1**.

4. The distribution of weights are found to be normally distributed.

5. The huge increase in number of filters and different sized kernels did not help much.

6. **VGGNet-inspired 5-layered model, M2 is found to be model of choice**. It even outperformed a 7-layered Convnet with huge number of parameters. The convergence speed w.r.t. epochs is also comparable between M2 and M3.
