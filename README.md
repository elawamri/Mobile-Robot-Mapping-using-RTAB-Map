# Mobile-Robot-Mapping-using-RTAB-Map
## Introduction
In this project i will create a 2D occupancy grid and 3D octomap from a simulated environment using my own robot with the RTAB-Map package.

RTAB-Map (Real-Time Appearance-Based Mapping) is a popular solution for SLAM to develop robots that can map environments in 3D. RTAB-Map has good speed and memory management, and it provides custom developed tools for information analysis.

For this project we will be using the ```rtabmap_ros``` package, which is a ROS wrapper (API) for interacting with RTAB-Map.

![Selection_697](https://user-images.githubusercontent.com/105011124/171433194-5064e041-75c7-41e7-b210-68657b7238cc.jpg)
## Mapping Test
#### 1. First, launch the Gazebo world and RViz, spawn the robot in the environment:
```
$ roslaunch my_robot world.launch
```
#### 2. Then, launch the ```teleop``` node:
```
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
#### 3. Finally, launch your mapping node:
```
$ roslaunch my_robot mapping.launch
```
Navigate the robot in the simulation to create map for the environment! When you are all set, terminal the node and you could find your map ```db``` file in the place you specified in the ```launch``` file. If you did not modify the argument, it will be located in the ```/root/.ros/``` folder.





