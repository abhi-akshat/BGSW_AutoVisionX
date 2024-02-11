cmake_minimum_required(VERSION 3.27)
project(BGSW_AutoVisionX)
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
link_directories(${OpenCV_LIBRARY_DIRS})

set(CMAKE_CXX_STANDARD 17)

add_executable(BGSW_AutoVisionX main.cpp)
target_link_libraries(BGSW_AutoVisionX ${OpenCV_LIBS})
