# Facial_key_points_detection

In this repository I showed how to detect eyes, lips, mid point of nose. The dataset is from a competition on kaggel. This kind of model is very useful for AR apps. Like some funny face editor whuch detect the face or head and make some funny character.
<br>
The dataset consists of 2k image which was (96X96) dims. But it was not enough. So I used data augmentations to get more data. I performed horizental flip and random brightness augmentations which generates almost 6k variations. Then I used a neural net of 4 hidden layers and use resnet skip connection to get a better result. The model has more than 17M parameters to train. So make sure your machine has enough computation ability to complete the task (preferably GPU). I tried with some values of alpha, beta_1 and beta_2. But the default value gives a better result.
<br>
I added the dataset which is 65mb. Also after training I saved the model and share the weights as well as the trained model in .json. I deleted the .hdf5 format because of its lagre size. If you train the model you can generate and save it. The model has an accuracy of 74% in test set. Although it is not very good, the predictions are not too bad. If you want to try this, instructions are given in the notebook so that you can follow. Some theory is also mentioned in the notebook which may help you.
