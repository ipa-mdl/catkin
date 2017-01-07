cmake_minimum_required(VERSION 2.8.3)
project(set_definitions)
find_package(catkin REQUIRED)

list(APPEND ${PROJECT_NAME}_DEFINITIONS -DTHIS_IS_MY_EXPORTED_DEFINITION)

add_definitions(${catkin_DEFINITIONS} ${${PROJECT_NAME}_DEFINITIONS})

catkin_package()
