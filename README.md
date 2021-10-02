# Potato Disease Classification Using CNN

## Problem Statement
Farmers who grow potatoes are facing lot of economical losses every year because of various disease that can happen to a potato plant.

There are two common disease:
- Early Blight and Late Blight.

- Early Blight: It is caused by a fungus and Late Blight is caused by a specific micro-organism and if a farmer can detect these disease early and apply appropriate treatment then it can save lot of waste and prevent the economic losses.

The treatment for Late Blight and Early Blight are little different, so it is important that you accurately identify what kind of disease is there in that potato plant.

## Objective
To build a mobile application and web page , which we can give it to farmers and farmers, all they need to do is go their farm and just take a picture of the plant and the application will tell them whether the potato plant is healthy or it has one of these disease and behind the scene application will be using deep learning and Convolutional Neural Network.


# WebApp


# Demo
https://user-images.githubusercontent.com/72372136/135665033-49c169e3-7a4a-4ee6-b085-12d2153b3e86.mp4

# Technical Aspects

- Python 3.7 and more
- Important Libraries: tensorflow, sklearn, pandas, numpy, matplotlib & seaborn
- Front-end: HTML, CSS 
- Back-end: Flask framework
- IDE: Jupyter Notebook, Pycharm & VSCode 
- Deployment: Heroku, AWS

# How to run this app 

Code is written in Python 3.9.4. If you don't have python installed on your system, click here https://www.python.org/downloads/ to install.

- Create virtual environment - conda create -n myenv python=3.9.4
- Activate the environment - conda activate myenv
- Install the packages - pip install -r requirements.txt
- Run the app - python run app.py

# Workflow

## Data Collection

We need to collect images of a healthy potato plant leaf and the potato plant leaf which has Early Blight or Late Blight disease.

Here we have used Data of Poatato Disease available in Kaggle.

Dataset credits: https://www.kaggle.com/arjuntejaswi/plant-village

## Data Cleansing and Pre-processing
Here we have used tf data set and  Data Augmentation. Data Augmentation because we were not having enough diverse set of images. So we did rotation, fliping and adjusted contrast to create more training samples.

## Model Creation and Evaluation

- Image Classification Model using CNN.
- Used Maxpooling2D and Flatten layers to create CNN.
- Activation Function used are: RELU and SOFTMAX.
- Model performance evaluated based on accuracy and loss.
- On test data we get approximately 100% accuracy.
- Model saved on local desk.


## Model Deployment
The final model is deployed on Heroku using Flask framework.

## Training, Validation Accuracy and Validation Loss Curve
![training and loss curve_potato](https://user-images.githubusercontent.com/72372136/135632014-e29ab0f1-185a-47f2-89bb-c1a2e1cd2e2b.JPG)

## UI
- User Interface is a very simple one, with single page asking for image to be classified.
![Potato_UI_1](https://user-images.githubusercontent.com/72372136/135632335-832ae18c-1d8c-42de-8eb0-7d54c07fe63b.JPG)

- After selecting image for classification, we just need to click predict button.
![Potato_UI_2](https://user-images.githubusercontent.com/72372136/135632485-76650f01-09c0-4679-bb28-e82a6e3d565d.JPG)

- Classification result will be displayed as following.
![Potato_UI_final](https://user-images.githubusercontent.com/72372136/135632580-18aabfa0-180d-4766-b9e5-dbf442edaf76.JPG)

- User can also download sample image for reference.
![Potato_UI_3](https://user-images.githubusercontent.com/72372136/135632744-ea2f1021-0dd9-4d53-9262-8824e8ed1cfe.JPG)

# Author

Upendra Kumar: https://www.linkedin.com/in/imupendra/

# Help Me Improve

Hello Reader if you find any bug please consider raising issue I will address them asap.
