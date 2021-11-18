# Brain Tumor Radiogenomic Classification Based on EfficientNet-PytTorch-3D

Jiawei Zhao  
zhaojw@bu.edu  

Kaggle: RSNA-MICCAI Brain Tumor Radiogenomic Classification  
Goal: Predict the status of a genetic biomarker important for brain cancer treatment  
Link: https://www.kaggle.com/c/rsna-miccai-brain-tumor-radiogenomic-classification  

## overview
### EfficientNet
Convolutional Neural Networks (ConvNets) are commonly developed at a fixed resource budget, and then scaled up for better accuracy if more resources are available. A new scaling method that uniformly scales all dimensions of depth/width/resolution uses a simple yet highly effective compound coefficient. This method uses neural architecture search to design a new baseline network and scale it up to obtain a family of models, called EfficientNets, which achieve much better accuracy and efficiency than previous ConvNets.  
Open Source: https://github.com/tensorflow/tpu/tree/master/models/official/efficientnet

![image](https://user-images.githubusercontent.com/59852184/140584198-41980172-b5e2-40d7-821b-1fb4a4a803b4.png)
![image](https://user-images.githubusercontent.com/59852184/140584219-52dd4177-59e6-4e71-82fe-4ee6592a0793.png)
![image](https://user-images.githubusercontent.com/59852184/140584229-26dc857b-6118-4452-93a9-549361febda4.png)

### Dataset
#### train_labels.csv  
![image](https://user-images.githubusercontent.com/59852184/140585919-87aa2ecf-ceaf-4b05-8d95-b0d63f940886.png)  
BraTS21ID is the patient's Id, Class 0 refers to people who do not have the methylation of the MGMT promoter. Class 1 seems to be someone who has the methylation of the MGMT promoter.

#### Train data
Train data has FLAIR, T1w, T1wCE, and T2w, respectively.  
![image](https://user-images.githubusercontent.com/59852184/140586074-58cabec4-7814-48ff-b9ef-22e1d4ba756b.png)

#### dcm file
![image](https://user-images.githubusercontent.com/59852184/140586158-9f4c3358-b054-4180-b951-61506d4626b7.png)

The one with MGMT_value = 1
Visualize the person with gene methylation = people with favorable prognostic factors and strong predictors of responsiveness to chemotherapy
![image](https://user-images.githubusercontent.com/59852184/140586462-57b64823-8a16-4924-a819-7697c1b5cede.png)

