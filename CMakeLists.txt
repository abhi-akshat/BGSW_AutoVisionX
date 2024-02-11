cmake_minimum_required(VERSION 3.27)
project(BGSW2)
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})
link_directories(${OpenCV_LIBRARY_DIRS})

set(CMAKE_CXX_STANDARD 17)

add_executable(BGSW2 main.cpp)
target_link_libraries(BGSW2 ${OpenCV_LIBS})