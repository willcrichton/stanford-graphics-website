---
layout: publication
title: "Scanner: Efficient Video Analysis at Scale"
authors:
    - "[Alex Poms](http://www.cs.cmu.edu/~apoms/) CMU"
    - "[Will Crichton](http://willcrichton.net), Stanford"
    - "Pat Hanrahan, Stanford"
    - "[Kayvon Fatahalian](http://graphics.stanford.edu/~kayvonf/), Stanford"
venue: |
    ACM Transactions on Graphics, 36(4), Aug 2018
    Proceedings of ACM SIGGRAPH 2018
---

![]({{ "/assets/images/publications/scanner/banner.jpg" | relative_url }})

## Abstract

A growing number of visual computing applications depend on the analysis of large video collections.
The challenge is that scaling applications to operate on these datasets requires
efficient systems for pixel data access and parallel processing across large numbers of machines.
Few programmers have the capability to operate efficiently at these scales,
limiting the field's ability to explore new applications that leverage big video data.
In response, we have created Scanner, a system for productive and efficient video analysis at scale.
Scanner organizes video collections as tables in a data store optimized for sampling frames from compressed video,
and executes pixel processing computations, expressed as dataflow graphs, on these frames.
Scanner schedules video analysis applications expressed using these abstractions onto heterogeneous
throughput computing hardware, such as multi-core CPUs, GPUs, and media processing ASICs, for high-throughput pixel processing.
We demonstrate the productivity of Scanner by authoring a variety of video processing applications
including the synthesis of stereo VR video streams from multi-camera rigs,
markerless 3D human pose reconstruction from video,
and data-mining big video datasets such as hundreds of feature-length films or over 70,000 hours of TV news.
These applications achieve near-expert performance on a single machine and scale efficiently to hundreds of machines,
enabling formerly long-running big video data analysis tasks to be carried out in minutes to hours.

## Paper

[Download Paper]() (XX MB)

## Code

[Code on Github](https://github.com/scanner-research/scanner/)
