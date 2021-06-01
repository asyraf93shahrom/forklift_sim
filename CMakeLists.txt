cmake_minimum_required(VERSION 3.0.2)
project(forklift_sim)

find_package(catkin REQUIRED COMPONENTS
geometry_msgs
  roscpp
  rospy
  rviz
  std_msgs
  tf
  xacro
)


catkin_package()


#############
## Install ##
#############

foreach(dir config launch meshes urdf worlds)
  install(DIRECTORY ${dir}/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach(dir)

install(
  FILES urdf.rviz
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
