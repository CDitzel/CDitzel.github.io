---
layout: home
title: Sensor data fusion
description: Robust environment perception in adverse weather
background: /assets/img/dl.png
permalink: /
---

{: .alert .alert-info}
Project page for my latest paper [GENRADAR: SELF-SUPERVISED PROBABILISTIC CAMERA SYNTHESIS BASED
ON RADAR FREQUENCIES](https://cditzel.github.io/GenRadar/) is up. Please let me know what you think.

My passion is in the field of self-learning neural networks applied to low-level
sensor data, particularly radar signals. The basic idea is to let the algorithms
find patterns and correlations without explicit annotations or manual human
interference. This allows for the exploitation of an unprecedented amount of
information and makes the environment perception for autonomous systems,
especially in unfavorable conditions, more reliable.  <img
src="/assets/img/rd_cam_points.png" align="left" width="400px"/> To obtain the
sparse point cloud representation of discrete reflection centers that most
experts are familiar with, conventional radar processing performs a series of
laborious calculations depending on various estimates and prone to rejecting
vital details of the measurements. It is thus imperative, to collect the data as
close to the sensor as possible to retain a maximum of information and let the
neural algorithms extract the essentials on their own. The adjacent image shows
a dynamic scene in range-Doppler and camera depiction with superimposed radar
targets in red. As a case in point, the reflections of the fourth person in the
far right back, present in the original recording, were discarded somewhere
along the calculations and are absent from the high-level radar point cloud
representation. Relying on the lower-level frequency plots instead retains most
of the crucial information concealed within the data, including the fourth
reflector. Please have a look at my related projects below and contact me for
further details or scientific discussions.<br clear="left"/>
