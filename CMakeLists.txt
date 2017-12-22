cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

PROJECT(myproject)

find_package(gazebo REQUIRED)
include_directories(${GAZEBO_INCLUDE_DIRS})
link_directories(${GAZEBO_LIBRARY_DIRS})

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${GAZEBO_CXX_FLAGS}")

add_library(freefloating_gazebo_fluid2 SHARED
    src/freefloating_gazebo_fluid.cpp
    src/freefloating_gazebo_fluid.h
)

target_link_libraries(freefloating_gazebo_fluid2 ${GAZEBO_LIBRARIES})
