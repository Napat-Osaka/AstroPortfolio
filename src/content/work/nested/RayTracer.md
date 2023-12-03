---
title: Ray Tracer
publishDate: 2020-03-04 00:00:00
img: /assets/RayTrace-1.jpg
img_alt: Pearls of silky soft white cotton, bubble up under vibrant lighting
description: |
  We developed a simple ray tracing software for scientific flow simulation.
tags:
  - Computer Graphics
  - 3D Modeling
  - C++
---

### In Pursuit of Beauty
In the chaos of non-linearity, there lies a beauty cold and serene. I am amazed at how in this field even simple equations can birth mesmerizing and unpredictable behavior. On the contrary, I am captivated by the idea that even in the midst of chaotic flows, patterns emerge, resilient and unchanging. Charmed by the beauty and complexity of fluid dynamics, I joined a research group focused on fluid simulation, aspiring to deepen my comprehension of this captivating field and, one day, emulate its inherent beauty through my own hand.

### Configuration Matters
In contemporary fluid simulation, we grapple with extremely large data, often reaching tens of billions of floating-point data for mere seconds of results. This means that researchers usually rely on supercomputers for executing simulations, a reliance that pose a challenge to data visualization when it comes to analysis. These challenges stem from the fact that supercomputers are designed primarily for computation rather than visualization. Common issues include limited access to visualization libraries, the complexity of utilizing provided libraries through the command line, and even the absence of an X Server (in other words, supercomputers lack a monitor!). 

While some existing tools can alleviate these challenges, they often demand cumbersome configurations unfamiliar to many mechanical engineers (Ex. Kubernetes). Consequently, this project aims to develop a specialized visualization tool tailored for fluid simulation applications. Our objectives revolve around three primary goals:

- High Visual Quality: Striving for realism surpassing common standards in the field.
- Ease of Use: Designed to run on supercomputers with minimal IT expertise and uncomplicated environment settings.
- Efficiency Boost: Giving fluid simulation researchers a powerful tool that streamlines the previously cumbersome visualization process, boosting analysis efficiency.

![alt text](/assets/RayTrace-2.jpg)
<div align="center">
  Visualization of Flow Structure at High Re number using tools that are common in the field. S. Goto, Y. Saito, and G. Kawahara, Phys. Rev. Fluids 2, 064603 (2017).
</div>

### Chasing the Light
Based on the Ray Tracing Algorithm that revolutionized the movie industry in the 2000s and has made waves in the video game industry these last few years, I built a simple yet powerful rendering engine from scratch. By simulating the movement of photons and the interaction between them and different materials, the Ray Tracing Algorithm can create a visualization that approaches the realism of authentic photographs. This level of authenticity proves invaluable in the analysis of highly complex simulations, where visual clarity is of paramount importance. 
Moreover, while we are still working on UI to make the system more user-friendly, our tool is indeed already capable of running on the supercomputer without any major configurations. All done on a highly parallelized algorithm to take advantage of supercomputers' numerous cores (but still run on the CPU for the moment). This project has been praised by researchers in the field and I received a BPA award from the Japanese Society of Mechanical Engineers.

![alt text](/assets/RayTrace-3.jpg)
<div align="center">
  Visualization of the same screen using our Ray Tracing tool, the difference in realism is simply striking.
</div>

![alt text](/assets/RayTrace-4.jpg)
<div align="center">
  Side by side comparison of the result of our Ray Tracing tool (Left) and traditional tool (Right). 
  Simulation data from 阪口智律, Osaka University Goto Lab (2023).
</div>