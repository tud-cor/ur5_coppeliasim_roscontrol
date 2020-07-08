cmake_minimum_required(VERSION 3.0.2)
project(ur5_coppeliasim_roscontrol)

## Compile as C++11, supported in ROS Kinetic and newer
add_compile_options(-std=c++11)


find_package(catkin REQUIRED COMPONENTS
  roscpp
  )



catkin_package(
  #INCLUDE_DIRS include #LIBRARIES ur5_coppeliasim_roscontrol
  CATKIN_DEPENDS roscpp 
  ur_description
  ur5_moveit_config
  ur_gazebo
  coppeliasim_run

  #DEPENDS system_lib
  )


include_directories(
  ${catkin_INCLUDE_DIRS} 
  )


#add_library(${PROJECT_NAME}
#    )





