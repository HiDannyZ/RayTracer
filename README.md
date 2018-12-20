# RayTracer
![.](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/DScene2.png)
# Disclaimer!
  I am unfortunately not able to share this source code due to academic integerity. However, I am able to share the executable and media files, so any interested people are able to run the application themselves. 

The Program was written in C++ utilizing:
- Microsoft Visual Studios C++.
- OpenGL

# Animation made from Images rendered in RayTracer

# Contact for any Questions
- Danny Zhu
  - [Linkedin](https://www.linkedin.com/in/danny-zhu-8b6556119/),
  - chdannyzhu@yahoo.com
  
# Ray Tracing Intro

![.](https://github.com/HiDannyZhu/RayTracer/blob/master/Animation.gif)

# Features:
Scene1            |  Scene2
:-------------------------:|:-------------------------:
![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/DScene1.png)  |  ![](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/DScene2.png)

## ViewPlane
![.](https://github.com/HiDannyZhu/RayTracer/blob/master/Images/ViewPlane.png)
The Viewplane is a graphically way to represent 3D objects as 2D
To produce Perspective projections are used to produce images which look natural. When we view scenes in everyday life far away items appear small relative to nearer items.

## BackWard Raytracing


## Phong Illumination model


  
## Reflection
<p align="center">
  <img src="CatmullRomPic2.png">
</p>

## Refraction
<p align="center">
  <img src="CatmullRomPic.png">
</p>

Utilzing catmull-spline and conservation of energy, the camera follows the interpolated control points between 2 points (from 0 to 1 as indicated from the picture). We use these control points to help direct the camera's motion and its orientation by using it to calculate the overall velocity in the system depending on the level of height.


# How to Run the Program:
  Download the Project_2.rar
  
  KEEP ALL FILE NAMES THE SAME and the same order.
  
  Double-click Project2.exe. 


### How was the Animation made?
FFMPRG

   
# Source for Images and more info:
https://www.mvps.org/directx/articles/catmull/

catmullRom.pdf


# Resources utilized:

Textbook: Peter Shirley, et. Al. Fundamentals of Computer Graphics (4th Edition). A K Peters Ltd; (ISBN:1482229390).

Reference book: OpenGL Programming Guide: The Official Guide to Learning OpenGL, Version 4.5 with SPIR-V (9th Edition). OpenGL Architecture Review Board, Dave Shreiner, Jackie Neider, Mason Woo, Tom Davis. Addison-Wesley; (ISBN1482229390)

