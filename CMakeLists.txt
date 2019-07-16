cmake_minimum_required (VERSION 2.8)

project(features)

find_package(OpenCV REQUIRED)

include_directories(${OpenCV_INCLUDE_DIRS})


add_executable(features features.cpp)

target_link_libraries(features ${OpenCV_LIBS})
