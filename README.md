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


* Second to convert audio into its spectrogram and then passing it to the CNN layers followed by  fully            connected layers  to do the prediction  

<img width="400" align ="left" alt="screen shot 2017-11-21 at 12 35 28" src="images/Mfccs.jpeg"> 

<img width="300" align="right" alt="screen shot 2017-11-21 at 12 35 28" src="images/spectrogram.png">
  

