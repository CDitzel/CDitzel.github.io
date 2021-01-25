
# Crossmodal Self-supervised Learning with
I am working in the area of applied self-supervised Deep Learning, a subfield within the
ever so growing domain of artificial intelligence.

## The need for annotation-free algorithms
In many areas of application, labelled data is scarse to come by or virtually
infeasible to obtain due to financial constraints and/or time
limitations. Manual human-in-the-loop approaches in which highly-trained
individuals highlight relevant properties within the input data trying to
capture their essence are error-prone and deprive the neural algorithms of the
chance to find inherent patterns buried within the data.

![GitHub Logo](/content/boundingbox.png)
*Annotating raw sensor data is reckless*
Format: ![Alt Text](url)

Not only will a human being inevitably make mistakes in annotating streams of
data by hand, it also influences the subsequent methods by
 introducing human
biases thus steering the algorithm in a certain direction from the very beginning.

Finally there is the financial aspect. Most companies and research facilities
cannot afford to pay millions to employ an armada of experts to cumbersomely
annotate plethora of data points.

The outlined problems necessitate a more natural approach in which the neural
network is tasked with finding interesting properties and complex correlations
withtin the data by itself without relying on predefied target specifications.

## Relying on raw sensor data
There is yet another problem in using high-level annotated data as input to
neural machines, namely the exclusion of vital and possibly valuable
information. According to [information
theory](https://en.wikipedia.org/wiki/Information_theory) special care has to be
taken in order to avoid equivocation, i.e. the outflow of potentially essential
knowlege by capturing the data as close to the respective sensor as
possible.

![GitHub Logo](/content/boundingbox.png)
*Conditional entropy as defined in information theory*
Format: ![Alt Text](https://en.wikipedia.org/wiki/Conditional_entropy)

This allows to retain a maximum of information which otherwise would
have been either altered or discarded altogether by subsequent steps along the
individual sensor processing chain.
