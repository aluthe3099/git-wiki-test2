---
published: true
---
# How to Debug in ROS

## General Debugging:

Check to make sure a ROS topic is published:
```
rostopic list
```

Check to see what is being published on a ROS topic named topic_name:
```
rostopic echo /topic_name
```

## Commonly Encountered Errors:

roslaunch: [ ] is neither a launch file in package [ ] nor is [ ] a launch file name
* make sure you source the setup.bash file
* rospack find
    * can be used to find the absolute path to a package - if rospack cannot find the file there's an issue
    