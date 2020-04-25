# Traffic-Signal-Classification

This is a Deep Neural Network approach to do traffic sign recognition
* Establishing a reliable Traffic Sign Classification mechanism is a major step in our journey towards building semi-autonomous/autonomous driving systems.
* This post intends to explain an approach to solve the problem of traffic sign classification and I intend to build, train and deploy a deep learning network for traffic sign classification.

# Project Highlights:
* The traffic sign dataset that we will be working on is GTSRB — German Traffic Signs. 
* The approach used is deep learning.
* The type of neural network used is a Convolutional Neural Network (CNN) paired with a linear classifier.
* Python is the language used to program this.
* The complete source code is uploaded

# DataSet For Training And Testing:
The pickled dataset Of German Traffic sign Recognition containing color images split across labelled training, test and validation sets
https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign/download

# Creating The Directory:
* Clone the Repository to create the directory 
https://github.com/utkarsh7kar/Traffic-Signal-Classification

# Working with Project:
* The Directory must contain the data set above described.
* Launch the traffic_sign in jupyter notebook
* run the program and a model named Trained_model.h5 will be created.
* launch user file in jupyter notebook
* run the program and the gui will be prompted.

# Some highlights:
* Around 96% accuracy over the test set 
* Learning rate annealing, Dropout increment, batch size increase as accuracy increases
* Greedy best save implemented on validation accuracy being the criteria

# Project Description
# * Pre-Processing of Data 
* Pre-processing techniques include 
  1. Centering around mean globally
  2. Locally centering the image around the mean
  3. Normalizing using Standard Deviation
  4. Use Histogram Equalization
Training Data needs to be Scaled and Normalized , Extended , Also Augmented , Balanced. It is sufficient to scale and normalize the validation & test data
# * Model Training
* Use of complete augmented dataset where each image is perturbed 10 times using augmentation techniques with an intensity factor and minimum sample target over 15 epochs. 
* The hyperparameters are fixed using search epochs for a simpler dataset and 2 classes. 
* The final accuracy on the test set after training the model for 15 epochs is 93.20 %
# * Model Testing
* RBG images are Converted to grey scale and the highest probable image classified is displayed:
<p align="center">
  <img src="traffic_sign_approximation.png" width="1500"/>
</p>


