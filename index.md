
# Crossmodal Self-supervised Learning
I am working in the area of applied self-supervised Deep Learning, a subfield within the
ever so growing domain of artificial intelligence.

## The need for annotation-free algorithms
In many areas of application, labelled data is scarce to come by or virtually
infeasible to obtain due to financial constraints and/or time
limitations. Manual human-in-the-loop approaches in which highly-trained
individuals highlight relevant properties within the input data trying to
capture their essence are error-prone and deprive the neural algorithms of the
chance to find inherent patterns buried within the data.

![GitHub Logo](/content/boundingbox.png)
*Annotating raw sensor data is cost-intensive and time-consuming*
Format: ![Alt Text](url)

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

## Relying on raw sensor data
There is yet another problem in using high-level annotated data as input to
neural machines, namely the exclusion of vital and possibly valuable
information. According to [information
theory](https://en.wikipedia.org/wiki/Information_theory) special care has to be
taken in order to avoid equivocation, i.e. the outflow of potentially essential
knowledge by capturing the data as close to the respective sensor as
possible.

![GitHub Logo](/content/equi.png =250x20)
*Important information must not be neglected*
Format: ![Alt Text](https://en.wikipedia.org/wiki/Conditional_entropy)

This allows to retain a maximum of information which otherwise would
have been either altered or discarded altogether by subsequent steps along the
individual sensor processing chain.

## Crossmodal correspondence learning
The basic idea is to employ time-synchronized streams of two orthogonal sensor
types and use one modality to supervise the other and vice versa. This allows
for the mathematically consistent formulation of an auxiliary task which is
attempted to be solved by the neural network in order to facilitate
backpropagation and enable the learning process.

The ultimate goal is to reveal areas within the camera image which are most
likely to be the source of electromagnetic reflections thus establishing a close
correspondence between both modalities which can then be used further for
safety-relevant applications downstream.

![](/content/architecture.gif)
![](/content/data_repr.gif )
![](/content/res1.gif)
![](/content/res2.gif)
