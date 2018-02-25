cmake_minimum_required(VERSION 3.9)
project(GUIMessing)
set(CMAKE_AUTOMOC ON)

set(CMAKE_CXX_STANDARD 11)
find_package(OpenCV REQUIRED)
find_package(Qt5Widgets REQUIRED)

add_executable(GUIMessing main.cpp plusminus.cpp plusminus.h)
target_link_libraries(GUIMessing ${OpenCV_LIBS})
target_link_libraries(GUIMessing Qt5::Widgets)