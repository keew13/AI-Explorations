# Audio Classification
A short project demonstrating the use of Artificial Neural Networks in classifying Audio signals. [Librosa](https://librosa.org/doc/latest/index.html)  package is used for reading the audio files and extracting the Mel-Frequency Cepstrum Coefficients which are used as the features(Independent Variables) representing the audio.
__
## Dataset
The dataset for this project was taken from [Urban Sound Datasets](https://urbansounddataset.weebly.com/). There is provision for two datasets; the one used over here is [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html). It contains 8,732 audio files distributed over 10 classes, splitted over 10 folds. The class labels are as follows:
* air_conditioner
* car_horn
* children_playing
* dog_bark
* drilling
* enginge_idling
* gun_shot
* jackhammer
* siren
* street_music
Additionally metadata is provided which contains apt information about the location of each audio file, the timestamps(start and end) they were clipped from original audio. More details can be checked at the above link for the dataset.
