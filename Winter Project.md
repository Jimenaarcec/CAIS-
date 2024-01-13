Jimena Arce jimenaarcec@gmail.com 

I choose the project consisting of the ASL alphabet data set where I trained a model to classify the 29 different signs showed in the data set. This was the Computer Vision Multiclass Classification.

Dataset. For the data set that I choose was the one given to us for this specific example which was the ASL alphabet data set from kaggle. Images were resized to 256x256 pixels and center-cropped to 224x224 pixels in order for the model to receive a constant input size. Pixel values were normalized by using the mean and standard deviation which helps speed up the training process. 

Model: For my model I used a pre-trained ResNet50 Model in which I freezes the pre-trained layers so the model could focus on only training the final fully connected layer for the ASL alphabet classification. The freezing also helps to prevent overfitting. Then the code distinguished the training and testing inputs and phases and then in the training output the loss and accuracy for each epoch. Then my batch size I set it to 128 because I was having a lot of problems with the time that it was taking to run the epochs and as I increased the batch sizes it took less time so I did that so my code could run. 

Model Evaluation/Results: I choose to evaluate the model encompassing 2 epochs since it was taking a long time and was trying to debug my code. The model is trained using specific criterion and optimizer and at the end of each epoch, the evaluation matrix like the validation loss and accuracy were calculated as well as the training time for each epoch. 

These were the results 
Epoch [1/2]. Train loss 0.793. Val loss 0.362. Val acc 90.897. Took 567.829 seconds
Epoch took 567.828604221344
Epoch [2/2]. Train loss 0.156. Val loss 0.257. Val acc 92.678. Took 589.109 seconds
Epoch took 589.1095175743103


Discussion: 
1) the data set is very important in this task as crucial for the model training because for this type of project you need a diverse representation of the ASL gestures. It is important that the data set captures a variation of lighting, backgrounds and hand positions. In this case the data set was very large so it was accurate for the project. Then the model was a good choice for image classification but can always depend on the complexity of the gestures presented in the data. The training procedures are good given that it gives us the losses and accuracy. 
2) For social implications, this ASL recognition has significant potential in the social good for those individuals in the community with hearing impairments. This could contribute to accessibility and inclusivity of this community of people in the world. Some limitations could be the biases of the data sets and the different hand shapes, positions where the model could struggle to define the different variations. 
3) My next steps could be to explore different ways to expand the data and the diversity of the data so the model could be exposed to more variation and be more accurate. Also using other types of pre training models on even larger data sets and see if the performace is enhanced. Also collaborating more with the ASL community for the dataset making and the validation which could provide more accurate insights. 

For this project I used the help of a gaggle notebook cited below 
https://www.kaggle.com/code/julichitai/asl-alphabet-classification-pytorch/notebook
And also used the help of chat GBT 
