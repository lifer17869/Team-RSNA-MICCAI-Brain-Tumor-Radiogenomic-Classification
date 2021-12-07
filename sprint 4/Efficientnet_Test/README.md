# Test Evaluation of EfficientNet Model
Jiawei Zhao

## Previous Job
We trained the models of each MRI scan type and got 12 models totally.  
The models are as followed:  
![Screenshot from 2021-12-06 18-45-29](https://user-images.githubusercontent.com/59852184/144940435-6544b33d-ec7e-4c31-9599-0c748791fb6d.png)

## Test Preparation  
We seperated 50 files from the dataset as the testset of efficientnet model and decided to get the performance of each model.  
In this way, we will get 5 test result:  
1. Best performance in Flair models
2. Best performance in T1w models
3. Best performance in T1wCE models
4. Best performance in T2w models
5. Average performance of models from 1-4

## Test Progress

### Best performance in Flair models 
In 4 Flair models, their AUC are calculated as followed:

Predict: FLAIR-e1-loss0.693-auc0.500.pth FLAIR (50, 2)  
Validation ensemble AUC: 0.5000  
Predict: FLAIR-e2-loss0.691-auc0.441.pth FLAIR (50, 3)  
Validation ensemble AUC: 0.4179  
Predict: FLAIR-e8-loss0.682-auc0.561.pth FLAIR (50, 3)  
Validation ensemble AUC: 0.4831  
Predict: FLAIR-e5-loss0.685-auc0.576.pth FLAIR (50, 3)  
Validation ensemble AUC: 0.5958  

We can find that model FLAIR-e5-loss0.685-auc0.576.pth has the maximun AUC.  And its prediction result showed in the figure is:  
![Screenshot from 2021-12-06 18-52-21](https://user-images.githubusercontent.com/59852184/144941025-060b5015-a2a0-492c-bc74-35abd3846380.png)

### Best performance in T1w models

Predict: T1w-e1-loss0.706-auc0.500.pth T1w (50, 4)  
Validation ensemble AUC: 0.5000  
Predict: T1w-e4-loss0.693-auc0.498.pth T1w (50, 4)  
Validation ensemble AUC: 0.4026  
Predict: T1w-e2-loss0.694-auc0.500.pth T1w (50, 4)  
Validation ensemble AUC: 0.5000  

The best model in T1w has a AUC of 0.5, it's not a valuable model.  
![Screenshot from 2021-12-06 18-54-22](https://user-images.githubusercontent.com/59852184/144941246-688c2897-cd71-4241-a50e-075ce4396906.png)



### Best performance in T1wCE models  
Predict: T1wCE-e1-loss0.692-auc0.515.pth T1wCE (50, 5)  
Validation ensemble AUC: 0.4750  
Predict: T1wCE-e2-loss0.691-auc0.500.pth T1wCE (50, 5)  
Validation ensemble AUC: 0.4783  
Predict: T1wCE-e3-loss0.691-auc0.408.pth T1wCE (50, 5)  
Validation ensemble AUC: 0.4686  
Predict: T1wCE-e5-loss0.688-auc0.602.pth T1wCE (50, 5)   
Validation ensemble AUC: 0.4364  
Predict: T1wCE-e4-loss0.690-auc0.587.pth T1wCE (50, 5)  
Validation ensemble AUC: 0.5089 

Best model in T1wCE is T1wCE-e4-loss0.690-auc0.587.pth.  
![Screenshot from 2021-12-06 18-55-43](https://user-images.githubusercontent.com/59852184/144941369-273f046d-a5e6-4033-aa7e-7614215ddfde.png)



### Best performance in T2w models
Predict: T2w-e1-loss0.702-auc0.500.pth T2w (50, 6)  
Validation ensemble AUC: 0.5000  
Predict: T2w-e2-loss0.692-auc0.500.pth T2w (50, 6)  
Validation ensemble AUC: 0.5000  
Predict: T2w-e4-loss0.691-auc0.433.pth T2w (50, 6)  
Validation ensemble AUC: 0.5072  
Predict: T2w-e10-loss0.688-auc0.586.pth T2w (50, 6)  
Validation ensemble AUC: 0.5733  

Best choice of T2W:T2w-e10-loss0.688-auc0.586.pth  
![Screenshot from 2021-12-06 18-56-44](https://user-images.githubusercontent.com/59852184/144941452-7b2bfd92-3066-40a3-88ed-8ba1d9b7c8d9.png)

### Average performance of models from 1-4
We selected the best model from each MRI type, and got the average AUC of the sum of prediction result.  

Predict: T1w-e1-loss0.706-auc0.500.pth T1w (50, 7)  
Predict: FLAIR-e5-loss0.685-auc0.576.pth FLAIR (50, 7)  
Predict: T1wCE-e4-loss0.690-auc0.587.pth T1wCE (50, 7)  
Predict: T2w-e10-loss0.688-auc0.586.pth T2w (50, 7)  
Validation ensemble AUC: 0.6055  

We found that the average result has the maximum AUC from now on.  
![Screenshot from 2021-12-06 18-59-41](https://user-images.githubusercontent.com/59852184/144941697-9768eed6-6978-4960-852c-4dff9a2ac1ab.png)

In order to have a much better result, we dele the T1w-e1-loss0.706-auc0.500.pth model and try to predict by use other three models.
Finally, it got the same result of the previous one.  
Predict: FLAIR-e5-loss0.685-auc0.576.pth FLAIR (50, 8)  
Predict: T1wCE-e4-loss0.690-auc0.587.pth T1wCE (50, 8)  
Predict: T2w-e10-loss0.688-auc0.586.pth T2w (50, 8)  
Validation ensemble AUC: 0.6055  

![Screenshot from 2021-12-06 19-01-15](https://user-images.githubusercontent.com/59852184/144941794-70e5ff21-a252-458b-8eeb-240d7281d269.png)


## Performance of All models
![Screenshot from 2021-12-06 18-36-37](https://user-images.githubusercontent.com/59852184/144941986-dd639556-58a1-4709-9a67-57831fec0b34.png)  
We can find from the figure that the average result of all best models in each type will have a better performance. So we decided to select this model as our final model.
