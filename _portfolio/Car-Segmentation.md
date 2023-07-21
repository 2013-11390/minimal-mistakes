---
title: "Car Segmentation"
order: 9
excerpt: "Divide Car component by using Mask RCNN."
header:
  image: /assets/images/carMaskRCNN.PNG
  teaser: /assets/images/carMaskRCNN.PNG
sidebar:
  - title: "Role"
    text: "Deep Learning Engineer"
  - title: "Task"
    text: "Divide car componets for getting the part of area."
  - title: "Stack"
    text: "Tensorflow, keras, anaconda"
gallery:
  - url: /assets/images/carMaskRCNN.PNG
    image_path: assets/images/carMaskRCNN.PNG
    alt: "result image1"
---

This is and example application of Mask RCNN for detecting tyre, light, number plate and grill of ther car using Keras. We use mask_rcnn_coco.h5 from release page and transfer learning by using it.  
This is term project for Project1 lecture in Seoul Nat'l University.

{% include gallery caption="This is a result for segmentation." %}

You can get code for this application in [here](https://github.com/2013-11390/splitCarCompByMaskRCNN)