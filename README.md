# PyTorch-YOLOv3
Brief introduction
Digits Detection:
This task is to train a network that can detect Street View House Numbers. The SVHN dataset is used for training. The training data has 33402 images and the testing data has 13068 images. The network trained this time is not only highly accurate, but also fast enough. The end result is that when a street view digital image is input, the network can output the predicted number and frame the number using bounding box.


## Installation
##### Clone and install requirements
    $ git clone https://github.com/eriklindernoren/PyTorch-YOLOv3
    $ cd PyTorch-YOLOv3/
    $ sudo pip3 install -r requirements.txt

##### Download pretrained weights
    $ cd weights/
    $ bash download_weights.sh

##### Download COCO
    $ cd data/
    $ bash get_coco_dataset.sh
    
