---
layout: publication
title: "Scanner: Efficient Video Analysis at Scale"
authors:
    - Alex Poms, CMU
    - Will Crichton, Stanford
    - Pat Hanrahan, Stanford
    - Kayvon Fatahalian, Stanford
venue: |
    ACM Transactions on Graphics, 36(4), Aug 2017
    Proceedings of ACM SIGGRAPH 2017
---

# Abstract

Modern game engines seek to balance the conflicting goals of high rendering performance and productive software development. To improve CPU performance, the most recent generation of real-time graphics APIs provide new primitives for performing efficient batch updates to shader parameters. However, modern game engines featuring large shader codebases have struggled to take advantage of these benefits. The problem is that even though shader parameters can be organized into efficient modules bound to the pipeline at various frequencies, modern shading languages lack corresponding primitives to organize shader logic (requiring these parameters) into modules as well. The result is that complex shaders are typically compiled to use a monolithic block of parameters, defeating the design, and performance benefits, of the new parameter binding API. In this paper we propose to resolve this mismatch by introducing shader components, a first-class unit of modularity in a shader program that encapsulates a unit of shader logic and the parameters that must be bound when that logic is in use. We show that by building sophisticated shaders out of components, we can retain essential aspects of performance (static specialization of the shader logic in use and efficient update of parameters at component granularity) while maintaining the modular shader code structure that is desirable in today's high-end game engines.

# Paper

[Download Paper]() (12 MB)

Shader components were implemented as an extension of the [Spire shading language](). You may also wish to see our SIGGRAPH [2016 paper]() on Spire.

# Code

[Code on Github]()
