# Task-02_Robot_arm
ROS packages that can be used to plan and execute motion trajectories for a robot arm in simulation and real-life.

These packages were tested under ROS kinetic and Ubuntu 16.04 and it works perfectly on ROS melodic

The robot arm uses Moveit plugin to apply kinematics by the KDL solver. These packages can be tested in the gazebo simulation tool and the real robot arm, where the ROS system and Arduino code share the /joint_states topic to control motors.
# Dependencies
run this instruction inside your workspace:
`mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/smart-methods/arduino_robot_arm.git 

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y`
For Ros Noetic:
`sudo apt-get install ros-noetic-moveit
 sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
 sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
 sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
# Robot Arm
The robot arm has 5 joints, 4 joints to connect the arm links where the last joint for the gripper.
## Circuit diagram



