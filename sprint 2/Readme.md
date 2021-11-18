A malignant tumor in the brain is a life-threatening condition. Known as glioblastoma, it's both the most common form of brain cancer in adults and the one with the worst prognosis. Detecting these tumors early in their life cycle will help patients to expand their expected life time. For detecting of these kinds of tumors in the brain with help of genetic marker is possible. One of these markers is genetic sequence with name of as MGMT promoter methylation has been shown to be a favorable prognostic factor and a strong predictor of responsiveness to chemotherapy.
But accessing to this marker needs special operation in the brains and opening skulls. Then it can take several weeks to determine the genetic characterization of the tumor. So, product mission of this work is creating a model to make this detection faster and more accurate without surgery. 

In last decade most of the Artificial intelligence tried to classify this tumor correctly. From 2012 to 2018 most of the algorithms tried to work with simple multi-layer perceptron and Supported Vector Machine (SVM) in recent years use of Convolutional Neural Network (CNN) for classification of tumors increased. 

For dealing with this task use of imaginary medical techniques is essential. Product mission of this work will be to creating an AI model which uses the input information from pictures to detect these tumors faster.  So, product mission will be:
1.	Gathering proper input data in form of pictures (MRI).
2.	Preprocessing pictures for accessing to the proper information for classification.
3.	Developing a Convolutional Neural Networks (CNNs) for dealing with this task.
4.	Testing proposed models based on test sets.
5.	Choosing best model.


# Architecture
The first part of the structure will be denoising and slicing. This chapter of the work have been defecated to first slicing of input pictures and eliminating the none essential and noisy picture. Then these pictures will go throw the process of feature selection. This process will be devoted extracting features for region of interest in the picture. This part is very important for gathering necessary information for replacing MGMT promoter methylation. 
Structure of the feature extraction can be done with:
1.	Convolutional Layer
2.	Genetic Algorithms
3. Histopathological features
4.
And other structure. Each of this procedure helps to extract potential features which then can be used for classification. Then these extracted features will go throw the model. The proposed model can be SVM, Bayesian network and deep learning. Deep learning model here can be with memory structure like RNN, GRU or LSTM. Other type of deep learning model which can be used here is different type of CNN like VGG16, VGG19, Resnet51, GoogLeNet, Mobile network and etc. Product architecture will be the model developing and testing developed model for the work.  

# User Story
User story will get divided to 2 phase: 1. Doctors 2. Patients.
Interest of these two groups of people in some phases are the same but in others they are different. Both of them wants to first classify the tumors in the brain easy and fast. Doctors wants to make sure that diagnosis is accurate enough so it is possible for them to demand for more survey so the Accuracy, specificity and sensitivity of classification is important. Segmentation of the tumors for gathering its location is very important for surgery.
Product Functions


Product function is simple like all of the artificial intelligence algorithms try to gather useful information for solving problem Glioblastoma classification. Result of classification here will be used to help doctors for better prediction and helping patients to get better treatment faster.


