cmake_minimum_required(VERSION 3.10.2)
project(mysample)

#bring the header files into the project
include_directories(include)

#manually add the sources using the set command below
set(SOURCES src/main.cpp src/function1.cpp src/function2.cpp)

#or allow for wildcard addition like
#file (GLOB SOURCES "src/*.cpp")

add_executable(mysample ${SOURCES})
install(TARGETS mysample DESTINATION bin)
