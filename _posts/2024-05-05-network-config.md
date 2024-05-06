---
published: true
---
# How to Debug Network Configuration Issues in ROS

Alright, when doing this you want to focus on a few things:
1. The /etc/hosts file
2. The ~/.bashrc file
3. The bash start files for startManualControl, startWirelessControl, startControl

## General setup

for /etc/hosts on BOTH machines

```
  127.0.1.1 rmccontrolstation
  127.0.1.2 rmctestbot
```

for ~/.bashrc
  on the control station, set:
  ```
    ROS_MASTER_URI=http://127.0.0.1:11311
    ROS_IP=127.0.0.1
  ```
  on the test bot, set:
   ```
    ROS_IP=127.0.0.1
   ```

## Testing
First test out the wired control
Make sure that roscore works, the file starts, and all pub/subs are working
If there's an error use roswtf (very useful to debug ip addr issues)

THEN test the wireless control
