# CarLogoTFLiteClassifier

### Overview

This is a camera app that continuously detects the car logo in the frames seen by your device's back camera, using a 
model trained. These instructions walk you through building and running the demo on an Android device.

### Want to create own model?

Here, we have trained our model to scan and detect car logo, but you can create your own custom model to create different categories objects. 

It has several steps to follow to create own custom model:

* First, you need to download this project and set up in Android Studio.
* Then, you need to open "https://teachablemachine.withgoogle.com/train" this link and add project for image detection.
* Next, add class for each of your object like here we have created class like BMW, Ferrari etc.
* Once, class will added successfully, we need to click on "Upload" button and upload all images that related to that class so our model can train and create model for that class
* We can upload multiple classes as per our requirements.
* When class adding process is completed, click on "Train model" button.
* It will take some time to train model. Once it trained, click on "Export Model" button.
* Now, we have option like Tensorflow.js, Tensorflow, Tensorflow Lite. Right now, we will choose "Tensorflow Lite" option.
* Under this selection, We have some options to select like Floating point, Quantized and EdgeTPU.
* Floating point will convert your model to floating point model and Quantized will convert your model to quantized model.
* We need to download model for both the options.
* Once, you have both model zip file then extract and replace model.tflite, moden_unquant.tflite and labels.txt with files in assets folder in our project.
* Now we are ready to scan and detect our objects.

