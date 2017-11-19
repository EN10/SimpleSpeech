# Speech Recognition

Based on: 
* [Simple Audio Recognition](https://www.tensorflow.org/versions/master/tutorials/audio_recognition)

## Install Tensorflow:

    sudo pip install -U pip  
    sudo pip install tensorflow 

## Test

[Test](https://www.tensorflow.org/versions/master/tutorials/audio_recognition#training_finished)

    cd test
    python label_wav.py \
    --graph=conv_actions_frozen.pb \
    --labels=conv_actions_labels.txt \
    --wav=a5d485dc_nohash_0.wav

## Pretrained Model

* [running_the_model_in_an_android_app](https://www.tensorflow.org/versions/master/tutorials/audio_recognition#running_the_model_in_an_android_app)
* [Pretrained Model v0.01](http://download.tensorflow.org/models/speech_commands_v0.01.zip)

## Train

[Training](https://www.tensorflow.org/versions/master/tutorials/audio_recognition#training)

    python train/train.py
    
## Keywords:

* "yes", 
* "no", 
* "up", 
* "down", 
* "left", 
* "right", 
* "on", 
* "off", 
* "stop", 
* "go", 
* silence, 
* an unknown word.