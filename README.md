# erwhi-hedgehog-ros
ERWHI Hedgehog ROS files

## Setup
Go into your workspace source folder (e.g. catkin_ws/src): <br>
`cd ~/catkin_ws/src` <br>
clone this repository: <br>
`git clone http://github.com/gbr1/erwhi-hedgehog-ros.git` <br>
return in catkin_ws: <br>
`cd ..` <br>
check dependencies: <br>
`rosdep install --from-paths src --ignore-src -r -y` <br>
make: <br>
`catkin_make` <br>
install: <br>
`catkin_make install` <br>

## Launch
Let's start Erwhi: <br>
`roslaunch erwhi_bringup bringup.launch` <br>
To simulate in Gazebo: <br>
`roslaunch erwhi_gazebo erwhi_gazebo.launch` <br>
To run autonomous navigation: <br>
`roslaunch erwhi_navigation explore.launch` <br>

## Demo
Video of robot working: [link to youtube](https://www.youtube.com/watch?v=5Fm99uoWtUY)<br>
Video of "How to Simulate Erwhi in Gazebo": [link to youtube](https://www.youtube.com/watch?v=R5mXczDg0mo)<br>

## Dependencies
* [sengi_ros](https://github.com/gbr1/sengi_ros)
* [bosch_imu_driver](https://github.com/gbr1/bosch_imu_driver)
* [realsense2_camera](https://github.com/intel-ros/realsense)

## Known issues
* _explore_ won't work with DWA, so Erwhi planners are based on TEB 
* frontier_exploration configurations need to be fixed.


__Copyright (c) 2019 Giovanni di Dio Bruno under MIT license__
