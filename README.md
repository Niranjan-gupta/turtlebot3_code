# turtlebot3_code

Clone this repository into your catkin workspace.
Clone the other packages needed to build in your repository
 git clone https://github.com/ROBOTIS-GIT/turtlebot3.git
 git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git
 git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git

Install these dependancies for turtlebot3:
sudo apt-get install ros-melodic-dynamixel-sdk

 Install this dependencies for melodic distro: (replace melodic with your distro)
sudo apt-get install ros-melodic-joy ros-melodic-teleop-twist-joy \
  ros-melodic-teleop-twist-keyboard ros-melodic-laser-proc \
  ros-melodic-rgbd-launch ros-melodic-depthimage-to-laserscan \
  ros-melodic-rosserial-arduino ros-melodic-rosserial-python \
  ros-melodic-rosserial-server ros-melodic-rosserial-client \
  ros-melodic-rosserial-msgs ros-melodic-amcl ros-melodic-map-server \
  ros-melodic-move-base ros-melodic-urdf ros-melodic-xacro \
  ros-melodic-compressed-image-transport ros-melodic-rqt* \
  ros-melodic-gmapping ros-melodic-navigation ros-melodic-interactive-markers
  
  Add the model that you are using to simulate: if its burger then use the below line 
  echo "export TURTLEBOT3_MODEL=burger" >> ~/.bashrc
  
  Build your workspace.
  To launch gazebo and rviz run:
  roslaunch simple_navigation_goals gazebo_navigation_rviz.launch 
  
  For point to point movement launch this file in another terminal:
  roslaunch simple_navigation_goals movebase_seq.launch
  
  
