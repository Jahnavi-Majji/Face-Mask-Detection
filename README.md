## Face-Mask-Detection
A deep learning model that detects whether a person has worn a mask or not, real-time.

#### Motivation
In the present scenario of the Covid-19 pandemic, wearing a face mask is much more important than everything to protect our lives. This face-mask detector helps you to check whether you have your protection mask on. 

This deep learning model can be extended to real-time detection using OpenCV and also as a telegram bot. The scripts for the use cases are included in the repo. 

![Web-cam](/real-time.jpeg)

The model was built using Transfer Learning which uses ResNet-50 as its underlying architecture. I have used the pretrained weights of the ImageNet model to train the network.

![conf-mat](/conf-mat.png)

The dataset consists of 3725 images with mask and 3828 images without mask with a total of 7553 images. Download the dataset [here](https://www.kaggle.com/omkargurav/face-mask-dataset)

#### Results

Metric | Result
--------|-------
Accuracy | 99.73
Training loss | 0.0086
Validation loss | 0.038

#### Requirements
* [FastAI](https://www.fast.ai/)
  * Check out their docs [here](https://docs.fast.ai/)
* [MobileNetV2](https://arxiv.org/abs/1801.04381)
* [OpenCV](https://opencv.org/)
* Tensorflow - Keras
