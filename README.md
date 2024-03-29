[![Maintenance](https://img.shields.io/badge/Developer-Danny_Zhu-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![Maintenance](https://img.shields.io/badge/Microsoft_Visual_Studios-C++-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
# RayTracer
![.](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/DScene2.png)
# Disclaimer!
The goal of this project was to build a program that takes a high-level description of a scene (where the objects, lights, and camera are) and produces the image seen through that camera.

The Program was written in C++ utilizing:
- Microsoft Visual Studios C++.
- OpenGL

# Animation made from Images rendered in RayTracer

![.](https://github.com/HiDannyZhu/RayTracer/blob/master/Animation.gif)
  
# Ray Tracing Intro
<p align="center">
 <img src="https://github.com/HiDannyZhu/RayTracer/blob/master/Images/RayTraceIntoImage.png" width="600" height="400" >
</p>

In Computer Graphics, Ray tracing is a technique for generating an image by tracing the path of light through pixels in an image
plane and simulating the effects of its encounters with virtual objects. The technique is capable of producing a very high degree of visual realism, usually higher than that of typical scanline rendering methods, but at a greater computational cost. This makes ray tracing best suited for applications where the image can be rendered slowly ahead of time, such as in still images and film and television special effects, and more poorly suited for real-time applications like computer games where speed is critical. Ray tracing is capable of simulating a wide variety of optical effects, such as reflection and refraction, scattering, and chromatic aberration.

As indicated in the image above, I implemented this program utilizing the well-known concept of **Backwards Raytracing** where the initial ray comes from the eye. This is so my algorithm will not render unneeded objects in the scene as there may be objects that block the view of another object.

For example, there may be a cube on a desk. If I add another bigger cube in front of the cube facing the camera, we wouldn't be able to see the first cube as its blocked. By avoiding to render the unseeable objects in the scene, the program runs a lot faster and is more efficient than [forward raytracing](https://en.wikipedia.org/wiki/Ray_tracing_(graphics)).

# Features:

## ViewPlane
![.](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/ViewPlane.png)
To be able to see the images created by the Ray tracer, I had to implement a view plane for our eye camera. Similar to how a camera creates 2D images from pictures on our 3D world, the Viewplane is a graphical way to represent 3D objects in a 2D plane.


## Phong Illumination model

No Lights            |  Lighted Sphere                       
:-------------------------:|:-------------------------:|
![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MySingleTriangleNoLight.png)  |  ![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MySingleSphereLighted.png)|

No Lights With Texture          |  With Texture and Light                      
:-------------------------:|:-------------------------:|
![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MytextureTriTest.png)  |  ![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MytextureSphereTest.png)|

  
## Reflection & Shadows
<p align="center">
  <img src="https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MyreflectionTest.png" width="700" height="400" >
</p>

## Refraction
<p align="center">
 <img src="https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MyrefractionTest.png" width="700" height="400" >
</p>

## Reflection & Refraction
Reflection and Refraction       |  Reflective Spheres                 
:-------------------------:|:-------------------------:|
![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MyreflectiveSpheres%26Tris.png)  |  ![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/Myreflection%26refraction.png)|

## Images made by myself
Scene1            |  Scene2
:-------------------------:|:-------------------------:
![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/DScene1.png)  |  ![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/DScene2.png)

## Tests Everything
![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/MytestEverything.png)

# How was the Animation made?
After rendering 76 frames by hand, I utilized ffmpeg to create the gif. 

   
# Source for Images/Textures and more info:
https://www.solarsystemscope.com/textures/

Badges:https://github.com/Naereen/badges

https://cs.stanford.edu/people/eroberts/courses/soco/projects/1997-98/ray-tracing/types.html

# Resources utilized:

Textbook: Peter Shirley, et. Al. Fundamentals of Computer Graphics (4th Edition). A K Peters Ltd; (ISBN:1482229390).

Reference book: OpenGL Programming Guide: The Official Guide to Learning OpenGL, Version 4.5 with SPIR-V (9th Edition). OpenGL Architecture Review Board, Dave Shreiner, Jackie Neider, Mason Woo, Tom Davis. Addison-Wesley; (ISBN1482229390)

