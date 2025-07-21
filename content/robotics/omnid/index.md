---
title: "Collaborative Manipulation"
summary: "The final goal of this project is to control a group of three omnidirectional robots to move some heavy objects together. There are two parts to this robot. The top half part of this robot is a delta robot, which is used to withstand some heavy objects. The bottom half part of this robot is an omnidirectional mobile robot with four mecanum wheels."
date: 2021-12-01
tags:
  - Mobile Robot
  - C++
  - ROS 1 
  - Navigation
  - OpenCV
  - Linux
url_code: 'https://github.com/pijuanyu/t265_pkg'
---
## Demonstration

{{< youtube id="014SftFy5WY" title="Formation Control Demonstration" >}}

{{< youtube id="nVxHEVh_cFk" title="SLAM Demonstration" >}}

## Project Overview

The final goal of this project is to control a group of three omnidirectional robots to move some heavy objects together. There are two parts to this robot. The top half part of this robot is a delta robot, which is used to withstand some heavy objects. The bottom half part of this robot is an omnidirectional mobile robot with four mecanum wheels.

I focus on the bottom part of the robot. And my project can also be divided into two parts. The first part is related to computer vision and navigation. The second part is about formation control to control a group of three robots. I use C++ to develop the first part and python for the second part.

**🔗 [View Source Code on GitHub](https://github.com/pijuanyu/t265_pkg)**

## Part 1

For the first part, the purpose of the first part is to use the Realsense T265 camera to do visual SLAM and navigation for one robot. This device is fascinating. Because it can provide an odometry frame and camera pose frame. That means we can get the location of this camera. Besides, it has a stereo fisheye camera. Compare with the normal camera, it has a wide-angle of view. And that will be much useful for detecting obstacles.

### Step 1: Apriltag detection

The first step is to connect T265 camera with the robot and test it with some April tags. I install this camera on the robot and successfully use it to track some apriltags. I can get the ID, position and orientation of the apriltag. And there is a realsense_ros package. When I launch the camera, I can get some rostopics of T265 camera.

{{< youtube id="LBJLwyytPmg" title="Apriltag Track Demonstration" >}}

### Step 2: Undistort the stereo fisheye camera

The second step is to undistort the stereo fisheye camera. If I need to use the stereo fisheye camera to detect some obstacles or build 3D map, I have to undistort it. I firstly do the camera calibration with OpenCV. I use ROS to subscribe to two fisheye images. Then I use approixamtetime approach to synchronize the left and right image messages. After that, I use the function from OpenCV to undistort the fisheye images and publish the undistorted image.

### Step 3: Obtain disparity map and 3D point cloud

The third step is to use undistorted images to calculate the disparity map and 3D point cloud. The disparity map is the pixel difference between a pair of stereo images. I also use the function of the OpenCV package to compute the disparity map. And according to the dispariy map, I calculate the 3D point cloud based on the functions.

{{< youtube id="70V8ewJPGXY" title="3D Point Cloud Demonstration" >}}

### Step 4: SLAM and navigation

The fourth step is to use octomap ros package to build 3D occupancy map and 2d projected map based on the 3D point cloud. And then when I successfully get the 2D map, I can start to do the 2D navigation by using ROS Navigation Stack. For the navigation, I can directly locate the T265 camera. I have 3D Pointcloud. So, I use the move_base package and DWA local planner to complete the navigation. This is what I have done in the first part.

{{< youtube id="C3MyeMfMPVE" title="SLAM Demonstration" >}}

## Part 2

I develop two controllers, which are the leader-follower controller and virtual structure controller.

For the leader-follower controller, I choose one robot as a leader and the other two robots as followers. When I control the first robot, another two robots will follower the leader. The theory is that I use a dynamic model to connect these three robots based on the position and orientation of the three robots.

For the virtual structure controller, I choose a virtual point. And then the three robots will rotate and translate around this virtual point. That means I can consider these three robots as one robot. They will rotate and move at the same time.

This is a formation control demo. I used a virtual structure controller to control a group of three omnidirectional robots. These three robots can simultaneously translation and rotation around a point.

{{< youtube id="hIp-aWaN-Pk" title="Formation Rviz Demonstration" >}}

{{< youtube id="102DDBKeH4M" title="Formation Real Demonstration" >}}
