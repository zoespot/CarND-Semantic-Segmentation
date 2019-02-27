# Semantic Segmentation
Self-Driving Car Engineer Nanodegree Program Term3 Project 2

[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

My code utilized a Fully Convolutional Network (FCN) to label the pixels of road in images. The FCN architecture is as below. Skip layer from VGG layer 3, 4 and 7 are combined with upsampled 1x1 convolutional layers.

![fcn_architecture1](./fcn_architecture1.JPG)
![fcn_architecture2](./fcn_architecture2.JPG)

Hyperparameters are chose with balance with accuracy and efficiency. L2 regularizer(1e-3) are used for all layers. Keep_prob is set to 0.5, learning rate = 0.0001. batch_siz =5.
With epochs =1, loss = 0.235. When epochs =10, loss = 0.108. Finally we use epochs =50, loss = 0.01~0.02.

All the labeled plots are in plots folder. Majority of them are correctly labeled with road vs non-road.

Here are some examples:

![plot1](./plots/epochs_10/um_000049.png)  
![plot2](./plots/epochs_10/um_000005.png)  
