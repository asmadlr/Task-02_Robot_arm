# Task-02_Robot_arm
ROS packages that can be used to plan and execute motion trajectories for a robot arm in simulation and real-life.

These packages were tested under ROS kinetic and Ubuntu 16.04 and it works perfectly on ROS melodic

The robot arm uses Moveit plugin to apply kinematics by the KDL solver. These packages can be tested in the gazebo simulation tool and the real robot arm, where the ROS system and Arduino code share the /joint_states topic to control motors.
# Dependencies
run this instruction inside your workspace:
` mkdir -p ~/catkin_ws/src `

` cd ~/catkin_ws/ `

` catkin_make `

` cd ~/catkin_ws/src `

` git clone https://github.com/smart-methods/arduino_robot_arm.git `

` cd ~/catkin_ws `

` rosdep install --from-paths src --ignore-src -r -y ` 

For Ros Noetic:

`sudo apt-get install ros-noetic-moveit `
` sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui `
 ` sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher `
 ` sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control `
# Robot Arm
The robot arm has 5 joints, 4 joints to connect the arm links where the last joint for the gripper.
## Circuit diagram

![circuit](https://user-images.githubusercontent.com/108361853/182257065-c1c1ac00-a6a0-4df5-bcc7-05fa570f14e5.png)


## Robot initial positions

![positions](https://user-images.githubusercontent.com/108361853/182257094-8e09ce65-20a4-41e0-a993-7c15c4204121.png)


## Usage
` source ~/.bashrc `
at the end of the (bashrc) file add the follwing line
`(source /home/asma/catkin_ws/devel/setup.bash)`
then 
ctrl + o
` roslaunch robot_arm_pkg check_motors.launch `

![‏‏لقطة الشاشة (37)](https://user-images.githubusercontent.com/108361853/182257150-06d0a54a-0d4c-4d82-890b-4a4d8b96913b.png)


