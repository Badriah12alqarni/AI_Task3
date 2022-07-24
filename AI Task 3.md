# AI_Task3
# Install the robot arm package :
~~~~
sudo apt-get install ros-noetic-catkin
 
mkdir -p ~/catkin_ws/src
 
cd ~/catkin_ws/
 
catkin_make
 
cd ~/catkin_ws/src
 
git clone https://github.com/smart-methods/arduino_robot_arm.git 
 
cd ~/catkin_ws
 
rosdep install --from-paths src --ignore-src -r -y
 
sudo apt-get install ros-noetic-moveit
 
sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
 
sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
 
sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
 
sudo nano ~/.bashrc
 
at the end of the (bashrc) file add the follwing line 
but change it to you name
 
source /home/badriah/catkin_ws/devel/setup.bash
 
source ~/.bashrc
 
roslaunch robot_arm_pkg check_motors.launch
~~~~
# Task execution picture
<div>
<img src="https://user-images.githubusercontent.com/108167855/179424309-5a5b2e8a-e408-43b5-93af-843b5362778c.png" width="350" height="200">
</div>
