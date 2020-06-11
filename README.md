This repository was forked and then adapted for the needs to the task of railway traffic lights detection.
(https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)

This repo let's you train a custom image detector using the state-of-the-art [YOLOv3](https://pjreddie.com/darknet/yolo/) computer vision algorithm. For a short write up check out this [medium post](https://medium.com/@muehle/how-to-train-your-own-yolov3-detector-from-scratch-224d10e55de2). 

### Pipeline Overview

To build and test your YOLO object detection algorithm follow the below steps:
 1. [Sample](boX.py)
 	- Choose the images to the train the algorithm on
 2. [Training](/2_Training/)
 	- Download pre-trained weights
 	- Train your custom YOLO model on annotated images 
 3. [Inference](/3_Inference/)
 	- Detect objects in new images and videos

## Repo structure

+ [`2_Training`](/2_Training/): Scripts and instructions on training your YOLOv3 model
+ [`3_Inference`](/3_Inference/): Scripts and instructions on testing your trained YOLO model on new images and videos
+ [`Data`](/Data/): Input Data, Output Data, Model Weights and Results
+ [`Utils`](/Utils/): Utility scripts used by main scripts

### Requisites

The only hard requirement is a running version of python 3.6 or 3.7.
To speed up training, it is recommended to use a **GPU with CUDA** support. 

## Full Start (Training and Inference)

To train your own custom YOLO object detector please follow the instructions detailed in the three numbered subfolders of this repo:
- [`2_Training`](/2_Training/) and
- [`3_Inference`](/3_Inference/).

## License

Unless explicitly stated otherwise at the top of a file, all code is licensed under the MIT license. This repo makes use of [**ilmonteux/logohunter**](https://github.com/ilmonteux/logohunter) which itself is inspired by [**qqwweee/keras-yolo3**](https://github.com/qqwweee/keras-yolo3).

## Acknowledgements
Many thanks to [Niklas Wilson](https://github.com/NiklasWilson) for contributing towards making this repo compatible with Tensorflow 2.0.
