cmake_minimum_required(VERSION 3.10)

include("thirdparty/basalt-headers/cmake_modules/PreProjectWorkarounds.cmake")

project(basalt)

if(DEFINED ENV{ROS_VERSION})
   include(${CMAKE_CURRENT_SOURCE_DIR}/CMakeListsROS.txt)
else()
   message(ERROR "ROS_VERSION environment variable is not set!")
endif()
