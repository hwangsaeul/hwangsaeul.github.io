---
layout: default
---

# Ultra-Low latency video transport 

We are planning to build new streaming system for a cloud-based video surveillance service.
In the new system, Secure Reliable Transport (SRT) will be used as a base protocol to archive
the critical requirements; ultra-low latency, packet loss recovery. 
SRT is considered to meet these requirements, but it is not enough to integrate to the existing service,
or newly developing business model. Hence, this project aims to develop SRT based ecosystem to satisfy 
various requirements; high performance, high scalability, and 3rd-party friendly SDK.
The final goal is to implement whole software stacks from embedded system to user application.

![SRT Ecosystem concept](./assets/img/SRT-concept.png)


## Visualized Effort

<iframe width="480" height="270" src="https://www.youtube.com/embed/ibRuFMJGffQ?controls=0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

This video is compact visualization of our efforts from the beginning. We will try to keep updating every month.

```
$ gource \
        -1920x1080 \
        -s .2 --auto-skip-seconds .2 \
        --multi-sampling \
        --stop-at-end \
        --output-framerate 30 \
        --hide mouse,progress \
        --highlight-users \
        --output-ppm-stream - \
        combined.log  | \
        avconv -y -r 30 -f image2pipe -vcodec ppm -i - \
        -b 32768k hwangsaeul.mp4 
```
