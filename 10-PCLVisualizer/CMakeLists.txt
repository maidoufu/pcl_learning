cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(pcl_visualizer_viewports)

find_package(PCL REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (pcl_visualizer_demo src/pcl_visualizer_demo.cpp)
target_link_libraries (pcl_visualizer_demo ${PCL_LIBRARIES})
