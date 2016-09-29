---
layout: default
title: Nationally Available Accelerated Computing Training
permalink: /training/
---

The following national training is currently available. If you would like to add training to the calendar then either [contact](contact) us or submit a pull request.

<br/>

{% for i in site.data.training %}
{% if i.archived == 'no' %}
#### {{ i.name }} ({{ i.location }}) ####
**Instructor:** *{{ i.person }}*

**Date:** *{{ i.date }}*

**Link:** <a href="{{ i.url }}">{{ i.url }}</a>

<br/>
{% endif %}
{% endfor %}


## Free Local NVIDIA GPU Training Courses Available ## 

If you are interested in receiving free training on GPU computing with NVIDIA GPUS then NVIDIA are able cover the costs of a limited number of 2 day training courses on "Introduction to CUDA" and "Deep Learning with DIGITS". You should contact [Anthony Morse](mailto:anthony.morse@icloud.com ) or [Paul Richmond](http://paulrichmond.shef.ac.uk/contact/) to arrange in first instances to arrange course at your instition.

Current NVIDIA courses are listed on the [European Training Calendar](http://www.nvidia.co.uk/object/cuda-training-calendar.html)


