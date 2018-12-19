# RayTracer
# Prototype-RollerCoaster

# Disclaimer!
  I am unfortunately not able to share this source code due to academic integerity. However, I am able to share the executable and media files, so any interested people are able to run the application themselves. 

The Program was written in C++ utilizing:
- OpenGL
- Microsoft Visual Studios C++.
# Video
[![YouTubeThumbNail](https://github.com/HiDannyZhu/Prototype-RollerCoaster/blob/master/YouTubeThumbNail.png)](https://www.youtube.com/watch?v=FFaznvya36A "Everything Is AWESOME")

# Contact for any Questions
- Danny Zhu
  - [Linkedin](https://www.linkedin.com/in/danny-zhu-8b6556119/),
  - chdannyzhu@yahoo.com
  
# Ray Tracing Intro

# Features:

## SkyBox

The roller-coaster is contained in a skybox: a cube with textures of ground,horizon, and sky that fit together to appear as a seamless large environment. To give my skybox a more realistic effect of being infinitely far away, I had it unaffected by the translation of the camera. Thus, no matter how far I moved, the skybox will never get closer.
  
## Track
<p align="center">
  <img src="CatmullRomPic2.png">
</p>

Catmull-Rom splines have C^1 continuity, local control, and interpolation. They are fantastic in ensuring C^1 continuity and having smooth curves. The Catmull-Rom spline essentially functions by taking 4 points and giving back positions from the interpolation between the 2nd and 3rd points where the starting position would be the integer 0 at the 2nd point and ending position would be the integer 1 at the 3rd point. With this, I stored these positions to shape the curve and track itself.

To create the track itself, I modified a track file containing a collection of control points that the track will go through. 

## Camera Control
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

   
# Source for Images and more info:
https://www.mvps.org/directx/articles/catmull/

catmullRom.pdf


#  Preamble

Press T to get on the track and press again to get off track

Press the U,I,O to increase transformations

Press the J,K,L to decrease transformations

Shift+Key will alter scale

Control+Key will alter translation

Key along will alter rotation rate

Pressing Comma will increase transformation Step

Pressing Period will decrease transformation Step

Pressing G will reset transformations

Pressing Q will toggle Quaternion Rotation

Pressing B will toggle reflections for the box textures

Pressing H will toggle heightmap

Pressing N will toggle Normals

Pressing P will print information

