# Visual Recognition using Deep Learning Homework 3
Brief introduction
Digits Detection:
This task is to train a network that can detect Street View House Numbers. The SVHN dataset is used for training. The training data has 33402 images and the testing data has 13068 images. The network trained this time is not only highly accurate, but also fast enough. The end result is that when a street view digital image is input, the network can output the predicted number and frame the number using bounding box.


## Reference:
    https://github.com/eriklindernoren/PyTorch-YOLOv3
## Reference:

$ git clone https://github.com/eriklindernoren/PyTorch-YOLOv3
$ cd PyTorch-YOLOv3/
$ sudo pip3 install -r requirements.txt

$ cd weights/
$ bash download_weights.sh

$ cd data/
$ bash get_coco_dataset.sh

$ python3 test.py --weights_path weights/yolov3.weights
$ python3 detect.py --image_folder data/samples/
$ python3 train.py --data_config config/coco.data  --pretrained_weights weights/darknet53.conv.74


$ cd config/                                # Navigate to config dir
$ bash create_custom_model.sh <num-classes> # Will create custom model 'yolov3-custom.cfg'
$ python3 train.py --model_def config/yolov3-custom.cfg --data_config config/custom.data
Add --pretrained_weights weights/darknet53.conv.74 to train using a backend pretrained on ImageNet.
