# Arm-Package-Installation
AI Track in Smart Methods Internship

First Step:
Installing the catkin tool.
Commands:
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/ 
catkin_make

Second Step: 
Installing Arm Packages.

Commands:
cd ~/catkin_ws/src
sudo apt-get install ros-noetic-moveit
sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

Third Step:
Start ROS
Commands:
cd ~/catkin_ws
catkin init
catkin_make

Get The arm files from smart methods:
git clone https://github.com/smart-methods/arduino_robot_arm

source /home/saud/catkin_ws/devel/setup.bash
roslaunch robot_arm_pkg check_motors.launch
