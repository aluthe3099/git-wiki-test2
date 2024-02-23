---
published: true
---
# Setting Up Basic Camera Functionality (imports, etc.)

Follow installation instructions [here](https://github.com/IntelRealSense/realsense-ros#installation-instructions)

For the basic purposes of demonstrating the ROS works with the intel realsense, we use [this](https://www.youtube.com/watch?v=eSAsLAzYzm4) video tutorial

From there, we were able to use the install bash file

We then used the following commands

* First terminal:
    * roscore
* Then in a second terminal:
    * roslaunch realsense2_camera rs_camera.launch
* Then in a third terminal:
    * rviz

This third terminal will open up the rviz terminal which then you go to add > by topic > /camera/color or /camera/depth and then SELECT IMAGE (camera and depth cloud do not display anything)


# Super Cool Intel RealSense + SLAM Stuff
Check this out [link](https://github.com/IntelRealSense/realsense-ros/wiki/SLAM-with-D435i), pretty cool method of getting and displaying a point cloud!
