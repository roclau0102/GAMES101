cmake_minimum_required (VERSION 3.20.3)

project(Rasterizer)

set(OpenCV_DIR "D:\\opencv\\build")
find_package(OpenCV REQUIRED)
find_package (Eigen3 REQUIRED)

set(CMAKE_CXX_STANDARD 17)

include_directories("D:\\opencv\\build\\include")
include_directories("C:\\Program Files (x86)\\Eigen3\\include")

add_executable(Rasterizer main.cpp rasterizer.hpp rasterizer.cpp Triangle.hpp Triangle.cpp)
target_link_libraries(Rasterizer ${OpenCV_LIBRARIES})
