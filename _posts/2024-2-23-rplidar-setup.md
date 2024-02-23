---
published: true
---

# General Info
RPLiDAR does a 360 degree view. Keep in mind this is basically just a flat plane of data (perhaps not the most useful for detecting craters and stuff)

# Before Starting
Keep in mind that part of the system (the words slamtec) will light up green when the USB-C cable is receiving enough power... If it isn't then your port won't show up when you run lsusb, and the lidar won't work

I also recommend looking through all the links a bit before starting working, since they all have different important bits of information to reference.

# Setting Up RPLiDAR
I used the following [YouTube tutorial](https://www.youtube.com/watch?v=Qrtz0a7HaQ4). Keep in mind you might need to run a different launch file than they demonstrate in the tutorial based on the RPLiDAR you use.

[This](https://github.com/robopeak/rplidar_ros) is also a good repository for setup, but the tutorial above includes important stuff like changing permissions on the port.

To run the UAV team's RPLIDAR (the one in the purple box that is an A3), you'll want to use the following commands

```
roslaunch rplidar_ros view_rplidar_a3.launch
roslaunch rplidar_ros test_rplidar_a3.launch
```

Right now, I haven't yet managed to get the rplidar_a3.launch launch file to pull up the visual within the rviz software


# TODO: update below info
To run the Lunabotics RPLIDAR (red box, a2 rplidar) you'll want to use the following:
