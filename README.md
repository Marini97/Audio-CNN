# CNN to classify audio files
This project is a CNN to classify audio files. It was developed as a final project for the course of Artificial Intelligence from Engineering to Arts at the University of Roma Tre.

## Description
The project use a simple CNN to classify audio files. The CNN is trained on the [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html) and on the [EMOVO](https://dagshub.com/kingabzpro/EMOVO) datasets. 

### UrbanSound8K
The dataset contains 8732 labeled sounds of urban sounds from 10 classes: 
- air_conditioner, 
- car_horn, 
- children_playing, 
- dog_bark, 
- drilling, 
- enginge_idling, 
- gun_shot, 
- jackhammer, 
- siren, 
- street_music. 
  
The classes are drawn from the urban sound taxonomy. For more details, [click here](http://www.justinsalamon.com/uploads/4/3/9/4/4394963/salamon_urbansound_acmmm14.pdf) for the paper.

### EMOVO
The dataset contains 588 labeled sounds built from the voices of 6 actors who played 14 sentences simulating 7 emotional states:
- dis: disgust
- gio: joy
- pau: fear
- rab: anger
- sor: surprise
- tri: sad
- neu: neutral



## Installation
### Clone the repository
```bash
git clone https://github.com/Marini97/Audio-CNN.git
```

### Install the required packages
It's recommended to use a virtual environment and then run the following command to install the required packages:
```bash
pip install -r requirements.txt
```

### Download the datasets
Download the datasets from the following links:
- [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html)
- [Emovo](https://dagshub.com/kingabzpro/EMOVO)

Before running the code, you need to set up the folder structure as described in the README files inside the folders 'Emovo' and 'UrbanSound8K'.

### Usage
Inside the folders 'Emovo' and 'UrbanSound8K' there are the following files:
- 'prep_dataset.ipynb': used to create the dataset of images for the CNN training.
- 'train.ipynb': used to train the model with k-fold cross validation.
- 'predict.ipynb': used to predict the class of a random audio file.



### Fix protobuf error
If you're getting the error: 
```
ImportError: cannot import name 'builder' from 'google.protobuf.internal' ...
```
You can fix it by copying the file 'builder.py' to your enviroment C:\ ... \Lib\site-packages\google\protobuf\internal