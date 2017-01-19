---
layout: project
type: project
image: https://github.com/cgyeager/hobby_pathtracer/blob/master/source/images/diffuse_reflect_refract.png
title: Hobby Pathtracer
permalink: projects/Pathtracer
date: 2016
labels:
  - Digital Image Synthesis
  - Computer Graphics
  - C++
summary: A small path tracer I developed over the summer.
---

<div class="ui small rounded images">
  <img class="ui image" src="https://github.com/cgyeager/hobby_pathtracer/blob/master/source/images/diffuse_reflect_refract.png">
</div>

This is a project implementing the path tracing algorithm that was used by Dr. Kajiya in the 1980s to approximate a solution to the rendering equation. It is basically a more general version of a ray tracer. A ray is cast from the camera into the scene and depending on the material the ray intersects it will reflect in a random direction. A new ray will then be cast from that hit point and detect another intersection (or not) in the random direction chosen. This will keep happening until the ray intersects with a light, the hemisphere above the scene in this case, or the depth of the recursive function is equal or greater than the max depth. This is what happens in the recursive function Radiance(). 

Before I started this project I read and implemented the ray tracer described in the book Ray Tracing from the Ground Up by Kevin Suffern to get a good understanding of the algorithm and also some of theory required to understand it. Afterward I read Advanced Global Illumination by Dutre et al. to gain a deeper understanding. 

If anyone is interested in learning more about ray tracing based algorithms I recommend [Scratchapixel](https://www.scratchapixel.com)
