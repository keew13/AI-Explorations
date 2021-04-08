# Audio Classification
A short project demonstrating the use of Artificial Neural Networks in classifying Audio signals. [Librosa](https://librosa.org/doc/latest/index.html)  package is used for reading the audio files and extracting the Mel-Frequency Cepstrum Coefficients which are used as the features(Independent Variables) representing the audio.

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

## Saved Models
Checkpoints were created during training and at every epoch the best models were saved. The models are present at [saved_models](https://github.com/keew13/AI-Explorations/tree/main/Audio%20Classification/saved_models).

## Explorary Data Analysis
A very basic EDA was performed for test samples and brief insights were collected. It can be found at [Basic Exploratory Data Analysis.ipynb](https://github.com/keew13/AI-Explorations/blob/main/Audio%20Classification/Basic%20Explorary%20Data%20Analysis.ipynb).

## Preprocessing and Training
Mel-Frequency Cepstrum Coefficients were extracted from each samples and were used for the classification puprose. They were inputted to a very shallow ANN which can be checked at [Preprocessing and Audio Classification.ipynb](https://github.com/keew13/AI-Explorations/blob/main/Audio%20Classification/Preprocessing%20and%20Audio%20Classification.ipynb).

## Directory Tree
Following is the hierarchy of folders as an additional information.
```
\---Audio Classification
    +---.ipynb_checkpoints
    +---saved_models
    \---UrbanSound8K
        +---audio
        |   +---fold1
        |   +---fold10
        |   +---fold2
        |   +---fold3
        |   +---fold4
        |   +---fold5
        |   +---fold6
        |   +---fold7
        |   +---fold8
        |   \---fold9
        \---metadata
```
### Note
Directory UrbanSound8K containing the dataset has not been uploaded to the repository due to its size. However its structure is as shown above in the Directory Tree.
