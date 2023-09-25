# navvis_description

## This is a ROS package that describes the navvis platform.
### Author: Zach Silberstein

#### Necessary installs

Both the gazebo_plugins and the velodyne_description packages are need.  

To install the gazebo_plugins package run:  
     `sudo apt install ros-<ros_version>-gazebo-plugins`

To install the velodyne_description package:  
    `sudo apt install ros-<ros_version>-velodyne-description`

#### Usage
To run the project, run the display.launch file by:  
    `roslaunch navvis_description display.launch`  
Default options are to run using the outdated robot.urdf file and to use the joint_state_publisher_gui.  
To run using the updated robot.xacro file:  
    `roslaunch navvis_description display.launch use_xacro:=true`
To use the joint_state_publisher instead of the joint_state_publisher_gui:  
    `roslaunch navvis_description display.launch use_gui:=false`
To run using the updated robot.xacro file and the joint_state_publisher:  
`roslaunch navvis_description display.launch use_xacro:=true use_gui:=false`