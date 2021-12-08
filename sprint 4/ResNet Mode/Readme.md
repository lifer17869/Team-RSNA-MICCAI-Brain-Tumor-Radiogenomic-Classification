In this part result of using Resnet model for classification of the tumors picture has been discussed. The result has been shown based on confusion matrix and Arear under ROC. 
 
Figure 1. Result of confusion matrix for binary classification.

 
Figure 2. Result of ROC for binary classification with Resnet. 
This result shows a bas classification for malignant tumor cancer. For benign tumors classification the result is better. Precision of achieved classification for benign tumors is 65%. But recall result of this part is 0.56 that shows bad true negative prediction.    
Result of training the model for 400 epochs has shown on Figure3.
 
Figure 3. Learning diagram of training for tumors classification.
•	Total number of pictures for training here is 19473 pictures.
•	Training samples have been furthermore divided to train set and validation. 
•	Batch size on each train set and validations is 1024.
•	Total number of epochs for training is 400 epochs.
•	Code have been implemented on 80K GPU.
•	Total runtime on GPU for training was 10 minutes and 50 second.
•	 Loss function is binary categorical cross entropy loss.
•	Optimization algorithms is Adam max.
The result of training and testing shows us that Resnet mode got overfitted. By overfitting structure, the test performance is less that training preperformance which make the. This problem comes with low number of epochs for training or low number of training set. Difficulty of relation between input and output is another problem. Also, structure of specific CNN model which will be used for classification has impact on overfiiting.

![image](https://user-images.githubusercontent.com/85686755/145240019-a7205608-feb1-42f6-9b43-334700accd48.png)

