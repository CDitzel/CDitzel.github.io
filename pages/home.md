---
layout: home
title: Radar perception & automotive security
description: Real-time radar processing, deep learning on low-level sensor data and secure embedded systems
background: /assets/img/web/banner2-banner.jpg
permalink: /
---

{: .lead}
I am a software engineer working on radar perception and automotive security.
During my doctoral research at Ulm University I developed self-supervised deep
learning methods that fuse low-level radar data with camera images. Since then I
have been bringing radar and deep learning into series production vehicles, from
a probabilistic radar grid running in real time on an embedded GPU to a
deep-learning model that detects obstacles and occupancy around the vehicle.
Today I work on embedded and automotive security: cryptographic key
provisioning, secure vehicle communication and diagnostics.

<div class="highlights row">
  <div class="col-md-4">
    <div class="highlight">
      <i class="fa fa-bullseye" aria-hidden="true"></i>
      <h3>Radar perception</h3>
      <p>Ten years of radar signal processing and deep learning on low-level radar data.</p>
    </div>
  </div>
  <div class="col-md-4">
    <div class="highlight">
      <i class="fa fa-microchip" aria-hidden="true"></i>
      <h3>Real-time embedded</h3>
      <p>CUDA on embedded GPUs, from the first prototype to series production.</p>
    </div>
  </div>
  <div class="col-md-4">
    <div class="highlight">
      <i class="fa fa-shield" aria-hidden="true"></i>
      <h3>Automotive security</h3>
      <p>Key provisioning, secure vehicle communication and diagnostics.</p>
    </div>
  </div>
</div>

## Research

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
