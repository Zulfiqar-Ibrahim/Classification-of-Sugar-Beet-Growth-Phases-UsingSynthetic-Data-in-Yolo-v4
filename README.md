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

<img src="Images/SugarBeet_stage_1.png" width="300" height="300">
