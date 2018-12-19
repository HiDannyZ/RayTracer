# RayTracer

# Disclaimer!
  I am unfortunately not able to share this source code due to academic integerity. However, I am able to share the executable and media files, so any interested people are able to run the application themselves. 

The Program was written in C++ utilizing:
- OpenGL
- Microsoft Visual Studios C++.

# Animation made from Images rendered in RayTracer
[![YouTubeThumbNail](https://github.com/HiDannyZhu/Prototype-RollerCoaster/blob/master/YouTubeThumbNail.png)](https://www.youtube.com/watch?v=FFaznvya36A "Everything Is AWESOME")

# Contact for any Questions
- Danny Zhu
  - [Linkedin](https://www.linkedin.com/in/danny-zhu-8b6556119/),
  - chdannyzhu@yahoo.com
  
# Ray Tracing Intro
My 2 images and 
# Features:

## ViewPlane

## BackWard Raytracing

## Phong Illumination model


  
## Reflection
<p align="center">
  <img src="CatmullRomPic2.png">
</p>

Catmull-Rom splines have C^1 continuity, local control, and interpolation. They are fantastic in ensuring C^1 continuity and having smooth curves. The Catmull-Rom spline essentially functions by taking 4 points and giving back positions from the interpolation between the 2nd and 3rd points where the starting position would be the integer 0 at the 2nd point and ending position would be the integer 1 at the 3rd point. With this, I stored these positions to shape the curve and track itself.

To create the track itself, I modified a track file containing a collection of control points that the track will go through. 

## Refraction
<p align="center">
  <img src="CatmullRomPic.png">
</p>

Utilzing catmull-spline and conservation of energy, the camera follows the interpolated control points between 2 points (from 0 to 1 as indicated from the picture). We use these control points to help direct the camera's motion and its orientation by using it to calculate the overall velocity in the system depending on the level of height.

## Basic Shading: Lighting of Normals
When light hits an object, an important fraction of it is reflected in all directions.
When a certain flux of light arrives at the surface, this surface is illuminated differently according to the angle at which the light arrives. If the light is perpendicular to the surface, it is concentrated on a small surface. If it arrives at a gazing angle, the same quantity of light spreads on a greater surface. This means that when we compute the colour of a pixel, the angle between the incoming light and the surface normal matters.

By accurately computing the normals of my track, the lighting on my track produced a very high degree of visual realism.

# How to Run the Program:
  Download the Project_2.rar
  
  KEEP ALL FILE NAMES THE SAME and the same order.
  
  Double-click Project2.exe. 


### How was the Animation made?


   
# Source for Images and more info:
https://www.mvps.org/directx/articles/catmull/

catmullRom.pdf


# Resources utilized:

Textbook: Peter Shirley, et. Al. Fundamentals of Computer Graphics (4th Edition). A K Peters Ltd; (ISBN:1482229390).

Reference book: OpenGL Programming Guide: The Official Guide to Learning OpenGL, Version 4.5 with SPIR-V (9th Edition). OpenGL Architecture Review Board, Dave Shreiner, Jackie Neider, Mason Woo, Tom Davis. Addison-Wesley; (ISBN1482229390)

