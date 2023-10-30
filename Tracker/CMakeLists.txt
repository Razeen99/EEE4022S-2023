cmake_minimum_required(VERSION 3.5)
 
project(tutorial-teabox-tracker)
 
find_package(VISP REQUIRED)
 
include_directories(${VISP_INCLUDE_DIRS})
 
add_executable(tutorial-mb-generic-tracker tutorial-mb-generic-tracker.cpp)
target_link_libraries(tutorial-mb-generic-tracker ${VISP_LIBRARIES})
