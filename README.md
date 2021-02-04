# DPhi-Datathon-Data-Sprint-22-Concrete-Crack-Image-Classification-
I achieved 9th rank in the recently held DPhi Datathon for Concrete Crack Image Classification where I achieved an accuracy of 99.902% in the test dataset. Here I 
will share my approach with how I did that. Everything has even been explained in the comments.The problem was solved on Google Colab.
<br>
The task was to train a model which could predict seeing the test images whether there was a crack in the image or not. 
<br>
The labels were given as Positive or Negative and I have converted them to 0(for negative) and 1(for positive). The grayscale image was converted into RGB format by stacking so 
that **VGG-16** and **ResNets** can be used to train the model. I converted the labels to dummies as is the general way to train Convolutional Neural Networks.The images were normalised 
so as to get an accurate model.
<br>
I trained VGG-16 and ResNetfor 10 epoches where the initial pretrained weights were left as it is and the later weights were trained.
<br>
VGG 16 performed better than the ResNet Model. Hence it was used to make predictions.I created a confusion matrix of validation data which showed excellent training results.
Later the model was made to predict on test dataset and the result implied 99.9024% accuracy. 
