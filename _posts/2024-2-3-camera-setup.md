---
published: true
---
# Setting up camera code

Follow installation instructions here: https://github.com/IntelRealSense/realsense-ros#installation-instructions

For the basic purposes of demonstrating the ROS works with the intel realsense, we use the following video tutorial: https://www.youtube.com/watch?v=eSAsLAzYzm4

From there, we were able to use the install bash file

We then used the following commands

First terminal:
roscore

Then in a second terminal:
roslaunch realsense2_camera rs_camera.launch

Then in a third terminal:
rviz

This third terminal will open up the rviz terminal which then you go to add > by topic > /camera/color or /camera/depth and then SELECT IMAGE (camera and depth cloud do not display anything)

