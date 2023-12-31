# Turtlebot3-with-SLAM
# Requirements
* Oracle VM VirtualBox Manager version 7.0
* Ubuntu-18.04.6-desktop-amd64.iso
* ROS melodic
# Install ROS on Remote PC
```
$sudo apt update
$sudo apt upgrade
$wget https://raw.githubusercontent.com/ROBOTIS-GIT/robotis_tools/master/install_ros_melodic.sh
$chmod 755 ./install_ros_melodic.sh 
$bash ./install_ros_melodic.sh
```
# Install Dependent ROS Packages
```
$ sudo apt-get install ros-melodic-joy ros-melodic-teleop-twist-joy \
  ros-melodic-teleop-twist-keyboard ros-melodic-laser-proc \
  ros-melodic-rgbd-launch ros-melodic-depthimage-to-laserscan \
  ros-melodic-rosserial-arduino ros-melodic-rosserial-python \
  ros-melodic-rosserial-server ros-melodic-rosserial-client \
  ros-melodic-rosserial-msgs ros-melodic-amcl ros-melodic-map-server \
  ros-melodic-move-base ros-melodic-urdf ros-melodic-xacro \
  ros-melodic-compressed-image-transport ros-melodic-rqt* \
  ros-melodic-gmapping ros-melodic-navigation ros-melodic-interactive-markers
```
# Install TurtleBot3 Packages
```
$ sudo apt-get install ros-melodic-dynamixel-sdk
$ sudo apt-get install ros-melodic-turtlebot3-msgs
$ sudo apt-get install ros-melodic-turtlebot3
```
# Set TurtleBot3 Model name
```
$ echo "export TURTLEBOT3_MODEL=waffle_pi" >> ~/.bashrc
```
# Execute Gazebo
```
$cd catkin_ws
$source devel/setup.bash
$export TURTLEBOT3_MODEL=waffle_pi
$roslunch turtlebot3_gazebo turtlebot3_world.lunch
```
![257977381-a136f6cd-be85-408f-9780-fe01d7715d21](https://github.com/ShahadAliH/Turtlebot3-with-SLAM/assets/145300172/72e2b3cc-5123-4dfa-9669-1868c8c1d148)
![ROS2](https://github.com/ShahadAliH/Turtlebot3-with-SLAM/assets/145300172/65fab1a5-3eaa-459b-80f7-a1a608b23f75)

