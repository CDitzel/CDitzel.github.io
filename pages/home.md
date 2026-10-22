---
layout: home
title: Sensor data fusion
description: Robust environment perception in adverse weather
background: /assets/img/dl.png
permalink: /
---

My passion is in the field of self-learning neural networks applied to low-level
sensor data, particularly radar signals. The basic idea is to let the algorithms
find patterns and correlations without explicit annotations or manual human
interference. This allows for the exploitation of an unprecedented amount of
information and makes the environment perception for autonomous systems,
especially in unfavorable conditions, more reliable.

To obtain the sparse point cloud representation of discrete reflection centers
that most experts are familiar with, conventional radar processing performs a
series of laborious calculations depending on various estimates and prone to
rejecting vital details of the measurements. It is thus imperative, to collect
the data as close to the sensor as possible to retain a maximum of information
and let the neural algorithms extract the essentials on their own.

<figure class="figure">
  <img src="{{ '/assets/img/rd_cam_points.png' | relative_url }}" class="figure-img img-fluid"
       alt="Range-Doppler map with three radar targets circled in red, next to a camera image of four people walking on a path">
  <figcaption class="figure-caption">
    A dynamic scene in range-Doppler (left) and camera depiction (right), with
    the radar point cloud targets superimposed in red.
  </figcaption>
</figure>

As a case in point, the reflections of the fourth person in the far right back,
present in the original recording, were discarded somewhere along the
calculations and are absent from the high-level radar point cloud
representation. Relying on the lower-level frequency plots instead retains most
of the crucial information concealed within the data, including the fourth
reflector.

Please have a look at my related projects below and contact me for further
details or scientific discussions.
