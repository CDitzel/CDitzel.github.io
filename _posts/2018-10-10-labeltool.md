---
title: ""
description: "Tesseract - A multimodal semi-automatic sensor data annotation tool for supervised learning"
background: /assets/img/labeltool.png
author: [Carsten Ditzel]
categories: [Sensor Fusion, Semantic Segmentation]
---

The vast majority of the annotated datasets used in research and academia lacks
any labeled radar data. Some collections include automotive radar information
but those are usually represented on a high-level by sparse point clouds, having
lost valuable information by preprocessing steps. This
[application](https://github.com/CDitzel/tesseract), written in modern C++,
OpenGL and Qt marks the attempt to classify low-level radar data in a similar
fashion to Lidar and Camera images. After semi-automatic projection of the Lidar
points into the camera image and assignment of the corresponding semantic
classes, those points vertical projection if used to assign unique class labels
to each range-azimuth cell of the radar cone. This work is by no means finished,
as it turned out that annotating radar frequency plots is far more involved than
initially anticipated. Also, the field of self-supervised learning seems to be a
more natural fire for domains in which labeled data are scarce or just hard to
come by. Nonetheless, the project contains many valid assumptions and showcases
a systematic approach how to obtain annotated radar plots for the purpose of
using them in the field of supevised learning.

![](/assets/img/labeltool2.png)
*Labeltool used to annotate real-world automotive radar frequency information*
