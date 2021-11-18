

Resent50 is one of most used CNN models which complies of 50 different layers and the structure of these layers has shown on the picture of the presentation. Instead of Using the forward simple connection Resent50 is using skip connection for better performance. Skip connection will help the model to get trained on the input data set better.  The different between our model and Resnet50 is the last layer which in original Resnet50 is consisted of 1000 neurons and the last layer of our model is consisted of only 2 neurons because we have 2 classes at the output. The structure of our model is consisted conv block and identity block which is clear at the middle and right side of the pictures.

In this slide specification for information first first convolution layer, batch normalization, pooling layer and conve layer has been mentioned.  For example, pictures input shape are 64*64*3 and first convolutional layer will change these shapes to 32*32*64 which means that number of filters on the pictures has increased to 64 from three ordinary channel of green, blue and red. Other specification about each layer specification can be seen in the page 3.

In this slid first on the left picture information about number of CNN model which had been the main algorithms for publication on the science journal has been mentioned here. This picture shows that number of publications from 2015 to 2020 has been increased rapidly and shows the vast majority use of CNN for different publications. Resnet 50 is one of the popular types of CNN so far which had been used so far [1]. The benefit of Using Resent has been mentioned on the left part. 


In machine learning and deep learning area we divide the input data set int 63% training, 7% validation and 30% testing. The main reason for this task is to make sure that our work is good. The most important result here is the test accuracy. In this page achieved result have been mentioned for better survey of the work and the training accuracy is 88% and validation accuracy is stock at 72%. The result of testing accuracy is 74% and the loss based on two class classification is 0.2. the out put prediction will be class 0 or class 1. Model actually tries to distinguish between different pictures base on input data. As it has been mentioned on the output prediction pictures most of the predicted outputs belongs to class 0 (800) and only 350 has been classified to class 1. All of the pictures in the data set are related to cancerous people. Based on their MGMT value if samples have been labeled by 0 it means that person has Benign tumor in their brains and the chance for progress in the tumor and make problem for functionality of the brain is low. But the label 1 means that the tumors in the brain is Malignant tumors and its patient must be treated as soon as possible in order to increase live expectation of patients. Main functionality of this work is to predict the Malignant tumors. 

Here explanation about the work and comparison between benefit of our model with other structure have been done. Most important explanation here is different between our model and the original Resnet 50. 


Reference
[1]. Dhillon, A., & Verma, G. K. (2020). Convolutional neural network: a review of models, methodologies and applications to object detection. Progress in Artificial Intelligence, 9(2), 85-112.

 



