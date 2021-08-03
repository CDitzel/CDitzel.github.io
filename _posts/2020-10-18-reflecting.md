---
title: ""
description: "Reflecting Objects: Which objects in the scene explain the radio frequency spectrum?"
background: /assets/img/refobjs-min.png
author: [Carsten Ditzel]
categories: [Self-supervised Learning, Sensor Fusion]
---


## Crossmodal Self-supervised Learning
I am working in the area of applied self-supervised Deep Learning, a subfield within the
ever so growing domain of artificial intelligence.

### Why radar matters
Radar offers many key advantages for modern autonomous vehicles. Particularly in adverse weather or compromised environment conditions does radar exhibit invaluable properties. When cameras and Lidar fails, radar still provides reliable estimates of obstables in the systems field of view.

![](/assets/img/fov.png)
*Radar offers complementary features to camera systems*


### The need for annotation-free algorithms
In many areas of application, labelled data is scarce to come by or virtually
infeasible to obtain due to financial constraints and/or time
limitations. Manual human-in-the-loop approaches in which highly-trained
individuals highlight relevant properties within the input data trying to
capture their essence are error-prone and deprive the neural algorithms of the
chance to find inherent patterns buried within the data.

![](/assets/img/boundingbox.png)
*Annotating raw sensor data is cost-intensive and time-consuming*

Not only will a human being inevitably make mistakes in annotating streams of
data by hand, it also influences the subsequent methods by
 introducing human
biases thus steering the algorithm in a certain direction from the very beginning.

Finally there is the financial aspect. Most companies and research facilities
cannot afford to pay millions to employ an armada of experts to annotate
plethora of data points.

The outlined problems necessitate a more natural approach in which the neural
network is tasked with finding interesting properties and complex correlations
within the data by itself without relying on predefined target specifications.

### Relying on raw sensor data
There is yet another problem in using high-level annotated data as input to
neural machines, namely the exclusion of vital and possibly valuable
information. According to [information
theory](https://en.wikipedia.org/wiki/Information_theory) special care has to be
taken in order to avoid equivocation, i.e. the outflow of potentially essential
knowledge by capturing the data as close to the respective sensor as
possible.

![](/assets/img/equi.png)

This allows to retain a maximum of information which otherwise would
have been either altered or discarded altogether by subsequent steps along the
individual sensor processing chain.

### Minimal processing of data retains valuable information
Only a minimum of preprocessing is performed on the data to retain as much information as possible inherent in the signals
![](/assets/img/data_repr.gif )

### Crossmodal correspondence learning
The basic idea is to employ time-synchronized streams of two orthogonal sensor
types then use one modality to supervise the other and vice versa. This allows
for the mathematically consistent formulation of an auxiliary task which is
attempted to be solved by the neural network in order to facilitate
backpropagation and enable the learning process.

![](/assets/img/architecture.gif)

The network is presented with temporally aligned and misaligned pairs of camera
and radar samples alternatingly. Upon transformation by means of two individual
encoder blocks, it then tries to bring matching samples closer
to each other in the high-dimensional embedding space, whereas the distance
between disparate sample pairs is to be increased simultaneously. This causes
the network to learn semantically meaningful representations of one and the same
real-world scene originating from orthogonal physical measurement principles.

![](/assets/img/local_outside.png)

The ultimate goal is to reveal areas within the camera image which are most
likely to be the source of electromagnetic reflections thus establishing a close
correspondence between both modalities which can then be used further for
safety-relevant applications downstream.

![](/assets/img/res1.gif)
![](/assets/img/res2.gif)
