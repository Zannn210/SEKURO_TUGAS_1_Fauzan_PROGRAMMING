cmake_minimum_required(VERSION 3.10)
project(robot)
#[TODO] Implentasikan CMakeList di bawah ini

#Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

#Set output executable ke bin
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY $(CMAKE_SOURCE_DIR)/bin)

#include file dari folder include/
include_directories(include)

#kumpulkan semua file .cpp
file(GLOB SOURCES "*.cpp")

#buat nama executable 'robot' 
add_executable(robot ${SOURCES})