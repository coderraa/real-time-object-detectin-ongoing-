# Real-Time-Object-Detection
@author *Rahul Singh*

YOLO algorithm
There are a few different algorithms for object detection and they can be split into two groups:

• Algorithms based on classification. They are implemented in two stages. First, they select regions of interest in
an image. Second, they classify these regions using convolutional neural networks. This solution can be slow
because we have to run predictions for every selected region. A widely known example of this type of algorithm
is the Region-based convolutional neural network (RCNN) and its cousins Fast-RCNN, Faster-RCNN and the
latest addition to the family: Mask-RCNN. Another example is RetinaNet.

• Algorithms based on regression – instead of selecting interesting parts of an image, they predict classes and
bounding boxes for the whole image in one run of the algorithm. The two best known examples from this group
are the YOLO (You Only Look Once) family algorithms and SSD (Single Shot Multibox Detector). They are
commonly used for real-time object detection as, in general, they trade a bit of accuracy for large improvements
in speed.

To understand the YOLO algorithm, it is necessary to establish what is actually being predicted. Ultimately, we aim to
predict a class of an object and the bounding box specifying object location. Each bounding box can be described using
four descriptors:

• center of a bounding box (bxby)

• width (bw)

• height (bh)

• value cis corresponding to a class of an object (such as: car, traffic lights, etc.).
In addition, we have to predict the pc value, which is the probability that there is an object in the boundingbox.

**We have used YOLOv5**

![object detection](https://user-images.githubusercontent.com/57325166/95173248-0ac4d680-07d6-11eb-8083-18e4fec46482.png)





