cmake_minimum_required(VERSION 3.10)
project(BezierCurve)

set(CMAKE_CXX_STANDARD 14)

set(OpenCV_DIR D:/openglrepo/opencv470)
find_package(OpenCV REQUIRED)

add_executable(BezierCurve main.cpp)

target_link_libraries(BezierCurve ${OpenCV_LIBRARIES})
