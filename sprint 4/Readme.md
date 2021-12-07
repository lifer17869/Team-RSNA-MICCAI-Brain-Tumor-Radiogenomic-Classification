# Evaluation of Two Models
In this step, we already got the models of Resnet and Efficientnet. After calculate the auc value, a better model will be selected.
Evaluation details of both methods are shown in each files.

## ROC of Resnet
![Screenshot from 2021-12-06 18-35-37](https://user-images.githubusercontent.com/59852184/144939617-55555cd0-b8af-4804-87a8-eb77e3ea9334.png)

## ROC of Efficientnet
Detail see : https://github.com/lifer17869/Team-RSNA-MICCAI-Brain-Tumor-Radiogenomic-Classification/tree/main/sprint%204/Efficientnet_Test  

![Screenshot from 2021-12-06 18-37-45](https://user-images.githubusercontent.com/59852184/144939755-c4ee399d-5328-42c8-b243-1301779267ac.png)

## Model Selection
Accoring to Rahaf's record the ResNet model needs nearly 10 hours to train the model, and the efficientNet modle Jiawei chose only takes a few hours. The AUC value of efficientNet is also bigger than ResNet's. Turns out we will select efficientNet as our final model.
