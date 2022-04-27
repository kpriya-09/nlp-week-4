# nlp-week-4
Speaker Identification using Neural Net.

Run the file in Google Colab

Epochs = 10
Accuracy ~ 98%
Speakers = 3
Dataset time = 10 mins

#Dataset
There are two options for the datasets. In either of the way you follow, download the dataset form Kaggle and keep the _background_noise_ & other folder for the Noise.

And pass the noise folder in the noise path while training and the same in the identification one too.

Kaggle dataset - https://www.kaggle.com/datasets/kongaevans/speaker-recognition-dataset

We recorded the speakers voice for 10 mins using the record.py file. And the obtained 10 mins .wav is then splitted into 1 seconds of wav files using audio_clip.py.

And then append the 1 second wav files into the data-set folder with the user name.

#Requirements

ipython == 7.31.1

numpy == 1.21.0 

pyaudio == 0.2.11

pydub == 0.24.1

tensorflow == 2.5.3

#Usage

#Training

Install the requirements

Download the Dataset or else create your own data set by speaking for 10 mins after running the file

python record.py

And split the generated data.wav into 1 second files using the audio_clip.py file.
Run python audio_clip.py

And train the neural net by running the the speaker-identification.ipynb file or run python speaker_identification.py

#Testing

After training, you will get the generated model.h5 locally in the root folder of the repo. And run python predict.py
