cmake_minimum_required (VERSION 3.20.3)
project (Transformation)

find_package (Eigen3 REQUIRED)
include_directories("C:\\Program Files (x86)\\Eigen3\\include")

add_executable (Transformation main.cpp)
