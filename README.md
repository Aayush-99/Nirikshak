# __NIRIKSHAK__

Nirikshak (derived from the hindi word "nirikshak" means Observer)is a tool that detects people in real time and returns a bounding box that turns red if the distance between two people is dangerously close.
This would help the authorities monitoring the potentially crowded areas to easily detect if social distancing protocols are being followed or not and necessary mesaures be taken to implement it.

![alt text](https://github.com/Aayush-99/Nirikshak/blob/master/Output.jpg "A frame from sample output")

## Table of Contents
* [General Info](#generalinfo)
* [Technology Used](#technology)
* [Detectron 2](#FAIR)
* [Further Improvements](#improvements)

## General Info
Social Distancing – the term that has taken the world by storm and is transforming the way we live. Social distancing has become a mantra around the world, transcending languages and cultures.
The biggest cause of concern is that COVID-19 spreads from person to person through contact or if you’re within close proximity of an infected person. Given how densely populated some areas are, this has been quite a challenge.
Nirikshak would help the authorities monitoring the potentially crowded areas to easily detect if social distancing protocols are being followed or not and necessary mesaures be taken to implement it.

## Technology Used
* PyTorch 1.5
* PyVision 0.6
* Detectron2
* OpenCV

## Detectron2
Detectron 2 is an open-source library for object detection and segmentation created by the Facebook AI Research team, popularly known as FAIR. Detectron 2 implements state of the art architectures like Faster R CNN, Mask R CNN, and RetinaNet for solving different computer vision tasks, such as:

* Object Detection
* Instance Segmentation
* Keypoint Detection
* Panoptic Segmentation

## Further Improvements
The projection of the camera matters a lot while computing the distance between objects in an image. In this case, I have not taken into account the projection of the camera since the impact of the camera’s projection on the estimated distance is minimum. However, the universal approach is to convert a video into a top view or birds’ eye view and then compute the distance between two objects in an image. This process is known as camera calibration. 

With more complex environments, it would be better to perform camera calibration, hence, this project can further be improved by using this technique.
