# About the Project

Aim of the project is to count number of people and their genders from a given Audio as mp3/wav file

## About the dataset

<img width="400" align="right" alt="screen shot 2017-11-21 at 12 35 28" src="https://user-images.githubusercontent.com/72940/33071669-be6c35b2-cebc-11e7-8822-9b998ad1ea09.png">

_CountNet_ is a deep learning model to estimate the number of concurrent speakers from single channel mixtures is a very challenging task that is a mandatory ﬁrst step to address any realistic “cocktail-party” scenario. It has various audio-based applications such as blind source separation, speaker diarisation, and audio surveillance.

[For more information about dataset, visit ](https://github.com/faroit/CountNet/blob/master/README.md)



## Problem Thinking 
**I followed two types of approahes to solve this problem:**


* First to extract mel-frequency cepstrum coefficients(Mfccs) features using librosa library and then passing them
    to the fully connected layers for prediction
* Second to convert audio into its spectrogram and then passing it to the CNN layers followed by  fully    connected layers  to do the prediction  


<img width="400" alt="screen shot 2017-11-21 at 12 35 28" src="images/Mfccs.jpeg">                 <img width="300" alt="screen shot 2017-11-21 at 12 35 28" src="images/spectrogram.png">





## Procedure
* First prepare the training data from the dataset by converting **.wav** file into mfccs features and **spectrograms** for the second model using librosa linrary
* Do the necessary preprocessing for both the models like resizing of images and reshaping into mfccs 
* Also add your own traning data by uploading audio files and preprocess and add the relevant labels
* Split data into training and testing dataset to check performace of model on unseen data
* Now choose the model architecures, loss function and the optimizer
* Choose the appropriate number of epochs, relevant callbacks such as early stopping 
* Evaluate the data on test data and on your  own audio by uploading it extract features and spectrogram and calling model.predict

## Model Architectures
<img width="400" alt="screen shot 2017-11-21 at 12 35 28" src="images/model.png">                 <img width="300" alt="screen shot 2017-11-21 at 12 35 28" src="images/Model.png">

## Test accuracy 
**Best test accuracy  was achienved by the second model using spectrograms of audio**
* Counting Male accuracy : **87%**
* Counting Female accuracy : **85%**
* Average accuracy : **86%**
  

