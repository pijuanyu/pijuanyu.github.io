---
title: "Quanticity Internship"
summary: "The purpose of this internship is to complete the basic autonomy of a ground vehicle. I will complete the SLAM and navigation based on LIDAR LD06, IMU, a depth camera and RGB camera. I used ROS2 galactic, OpenCV and Navigation2 to finish the whole project. Before running navigation in the physical robots, I will test these approaches in the Gazebo Simulation platform."
date: 2022-03-05
type: docs
tags:
  - Mobile Robot
  - Python
  - ROS 2 
  - Gazebo
  - Navigation
  - OpenCV
  - Linux
---
## Demonstration

This is a demo of SLAM. I use slam toolbox, ROS2 galactic and Gazebo to finish this demo. It can detect the obstacles and create a map of this maze world.

{{< youtube id="BVC1nPVfYOA" title="ROS2 SLAM Demonstration" >}}

## Project Overview

The purpose of this internship is to complete the basic autonomy of a ground vehicle. I will complete the SLAM and navigation based on LIDAR LD06, IMU, a depth camera and RGB camera. I used ROS2 galactic, OpenCV and Navigation2 to finish the whole project. Before running navigation in the physical robots, I will test these approaches in the Gazebo Simulation platform.

My tasks will be divided into these steps.

Step1: Transfer CAD files of the ground vehicle into a URDF file. Then import the URDF file into the Gazebo.

Step2: Setup differential drive plugin, Lidar plugin, depth camera plugin and IMU plugin in the URDF file so that it can publish “cmd_vel” and “Odom” rostopic.

Step3: Develop a controller so that PS4/Xbox controller can be used to drive the robot in the gazebo.

Step4: Create a static maze world in the gazebo. Use the slam toolbox and lidar to do the SLAM and build the map of this maze world.

Step5: Use navigaiton2 to finish the navigation with the map which is created by the SLAM (known environment)and the navigation without the map (unknown environment)

Step6: Build a dynamic world in the gazebo. Do the navigation of the mobile robot in a dynamic environment.