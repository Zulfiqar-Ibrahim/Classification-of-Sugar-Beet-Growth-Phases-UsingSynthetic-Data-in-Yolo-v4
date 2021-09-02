# Classification-of-Sugar-Beet-Growth-Phases-UsingSynthetic-Data-in-Yolo-v4
In  this  project,  classification  system  has  predicteddifferent  growth  phases  of  synthetic  images  of  sugar  beet  usingstate  of  an  art,  real-time  object  detection  model  (Yolo  v4).  Toachieve this task, Blender is used for the creation of sugar beet’s3D  models  and  Unreal  Engine  4  for  the  simulation  in  different environments. 

There are four types of 3D models according to their growth phase which is then placed in a simulated environment in Unreal Engine for the acquisition of images.
Unreal engine is used to simulate a farm-like environment for acquisition training images. This training data is used for the
training and validation process for Yolo net. In the end, 3D models of sugar beet in a simulated environment have produced
substantial results which proved that synthetic data can be used for real-life application of object detection.

In this project, state-of-the-art Yolo v4 net  was deployed
for the classification of the age of the sugar beet plant in
real-time. For training and validation purposes, four classes of
3D models of sugar beet were designed in Blender software
and deployed in an Unreal Engine environment with variable
weather settings. A camera is attached to the tractor in
a simulated environment which records the video of beets
planted in soil. Extracted images are labeled from the video
and feed them to Yolo net for training and validation processes.
The optimal goal of this project is to achieve the substantial
percentage of Mean Average Precision (m.A.P) in Yolo net by
using synthetic data.


To achieve this goal, pipeline is divided
this pipeline into IV parts. Part I is designated for the creation
of 3D models of sugar beets according to their age group.
In part II, these 3D models are placed into the Unreal Engine
farm environment. This simulation provides two sets of videos
where one video is in general RGB format and the second
video is in black and red segmented format. This pixel-wise
segmented format is provided by the Unreal engine. In part III,
original RGB image are labeled by using a segmented image,
through the OpenCV library. In part IV feed Yolo net with
these labelled images for the training and validation purpose.

## Project Pipe line 

This section discusses the complete pipeline of our project.
The first task in our pipeline is to create a 3D model of
sugar beet. These models are categorized according to their
age. there are four phases (0-4) for each 3D model. Blender
software is used for the modeling of these sugar beets. For the
textures of leaves, real texture is captured from a video of a
sugar beet farm. In this way, there is no need to create texture
from ground zero. These textures are then mapped to the leaf
model of the sugar beet to create a sense of realism. After
creating five models of sugar beet in Blender software, then
import the .fbx files of these models in the Unreal Engine 4
for farm simulation.
In Unreal Engine 4, farm simulation is designed with vari-
able weather. This simulation gives control over every detail
like weather, soil texture, plant spacing, air pressure, terrain
adjustment, etc. Tractor model is also constructed which will
drive from one point to other points in the field. The path
of tractor movement is selected by the user. After the path
selection, camera is attached to the tractor which will take
images of sugar beet planted in the soil. The parameters of a
camera will be discussed later.

<img src="Images/draw_io.png">

### Camera Setup


The camera is the most important component in this sim-
ulation which is used for the image acquisition of sugar beet
plants. The project mode of the imaging system is set as
”Perspective” and Field of View is set around 90 ◦ . The reason
for 90 ◦ is the capture most of the ground without the fish-
eye lens effect. The aspect ratio is set around 1.777 but it
can be changed according to requirements. This camera setup
provides sharp images of sugar beet planted in the soil. The
distance between soil and camera is around 1.5 meters.


### 3D models of Sugar Beet

To create a simulation in Unreal Engine, a 3D model of
sugar beet is designed in Blender. This is the best tool available
for 3D modeling and designing. With the help of this tool, 5
phases of sugar beet are created. These 5 phases are according
to their growth stages.


<img src="Images/SugarBeet_stage_1.png" width="300" height="300">

Phase 0 refers to the initial growth stage which is very
early in development. This stage has very small leaves and
a vertically longer beetroot.
