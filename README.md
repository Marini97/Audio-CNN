# CNN to classify audio files
This project is a CNN to classify audio files. It was developed as a final project for the course of Artificial Intelligence from Engineering to Arts at the University of Roma Tre.

## Description
The project use a simple CNN to classify audio files. The CNN is trained on the [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html) dataset. The dataset contains 8732 labeled sound excerpts (<=4s) of urban sounds from 10 classes: air_conditioner, car_horn, children_playing, dog_bark, drilling, enginge_idling, gun_shot, jackhammer, siren, and street_music. The classes are drawn from the urban sound taxonomy. For more details, see the paper [here](https://urbansounddataset.weebly.com/uploads/3/0/2/0/30205859/urbansound.pdf).

### Fix protobuf error
If you're getting the error: 
```
ImportError: cannot import name 'builder' from 'google.protobuf.internal' ...
```
You can fix it by copying the file 'builder.py' to C:\ ... \Lib\site-packages\google\protobuf\internal