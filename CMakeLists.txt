cmake_minimum_required(VERSION 3.10)
project(fisheye_calibrate)

set(CMAKE_CXX_STANDARD 14)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})



add_executable(fisheye_calibrate main.cpp)

target_link_libraries(fisheye_calibrate ${OpenCV_LIBS})