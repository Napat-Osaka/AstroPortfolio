---
title: GUI Development
publishDate: 2019-10-02 00:00:00
img: /assets/UI.jpg
vid: /assets/video/ui
img_alt: Soft pink and baby blue water ripples together in a subtle texture.
description: |
  Based on OpenGL and its rich supporting assets, we are building a GUI system for our in-house flow simulation visualizer.
tags:
  - Computer Graphics
  - C++
---

> OpenGL based software made to act as user-friendly UI, supporting my original Ray Tracer

\* iOS don't like auto play tag ! start the video manually if you are on iOS

### Good Old Trusty OpenGL
Ray Tracing, while renowned for its exceptional visual results, comes with a significant drawback—its speed, or rather lack thereof, compared to the much swifter Rasterization method. Waiting up to 15 minutes for the final visualization is usually acceptable, but the prolonged wait during adjustments is far from optimal. To address this, our supporting software, designed as a user-friendly GUI for fine-tuning visualization parameters before feeding them to the Ray Tracing System, is built upon the foundation of OpenGL.
Recognized as the standard library of Rasterization for decades, OpenGL is our go-to choice for its impressive speed and comprehensive toolset. By adopting OpenGL, we aim to expedite the adjustment process, providing users with a more responsive experience. The library's wealth of supporting tools also promises to streamline our workflow and enhance the overall user experience.

![alt text](/assets/UI-2.jpg)
<div align="center">
  A simple OpenGL visualization
</div>

### Undebugable Shaders
OpenGL's exceptional speed stems from its close collaboration with GPUs, optimizing essential computations. To harness this power, we must work with a special type of program known as shaders. These are the procedures meant for GPU that are done on the geometric data such as rotation (vertex shader), and lighting effect (fragment shader). After a lot of tutorials and an embarrassingly huge number of trials, I managed to make a workable set of shaders that can also take in additional textures, giving a good lighting effect on metalic surface. 

### GUI At Last
By integrating the powerful 3D visualization capabilities of OpenGL with the intuitive GUI Library Dear ImGui, we are in the process of developing a robust GUI system to support our primary Ray Tracer. This integration aims to streamline and expedite the setup process, making it more user-friendly and efficient. While it remains a work in progress, the top demo showcases the implementation of fundamental control functions, including color adjustments and movement.