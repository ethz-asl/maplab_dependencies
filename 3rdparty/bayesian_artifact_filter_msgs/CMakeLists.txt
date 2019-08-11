cmake_minimum_required(VERSION 2.8.3)
project(bayesian_artifact_filter_msgs)
find_package(catkin REQUIRED COMPONENTS
std_msgs
geometry_msgs
sensor_msgs
message_generation

)

#add_service_files(
#  DIRECTORY srv
#  FILES
#)

add_message_files(
  DIRECTORY msg
  FILES
  filtered_art.msg
)

generate_messages(
  DEPENDENCIES
  geometry_msgs
  sensor_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime geometry_msgs sensor_msgs
)
