cmake_minimum_required(VERSION 3.10)
project(Rasterizer)

set(CMAKE_CXX_STANDARD 17)

set(OpenCV_DIR D:/openglrepo/opencv470)
find_package(OpenCV REQUIRED)

include_directories(D:/openglrepo/Include)

add_executable(Rasterizer main.cpp rasterizer.hpp rasterizer.cpp Triangle.hpp Triangle.cpp)
target_link_libraries(Rasterizer ${OpenCV_LIBRARIES})