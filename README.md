# forklift_sim
this package provide simulation of forklift in rviz and gazebo

# clone package in catkin
$ cd catkin_ws/src
$ git clone https://github.com/asyraf93shahrom/forklift_sim.git

# Run the simulation (gazebo and rviz)
roslaunch forklift_sim forklift.launch

# open second terminal to run rqt for control
rqt

# Run the simulation (gazebo only)
roslaunch forklift_sim forklift_gazebo.launch
