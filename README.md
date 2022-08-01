# Task-02_Robot_arm
ROS packages that can be used to plan and execute motion trajectories for a robot arm in simulation and real-life.

These packages were tested under ROS kinetic and Ubuntu 16.04 and it works perfectly on ROS melodic

The robot arm uses Moveit plugin to apply kinematics by the KDL solver. These packages can be tested in the gazebo simulation tool and the real robot arm, where the ROS system and Arduino code share the /joint_states topic to control motors.
# Dependencies
run this instruction inside your workspace:
' mkdir -p ~/catkin_ws/src '


