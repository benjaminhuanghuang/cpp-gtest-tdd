cmake_minimum_required(VERSION 3.7)

set(This CMakeExample)
project(${This} C CXX)

set(CMAKE_C_STANDARD 99)
set(CMAKE_CXX_STANDARD 11)

enable_testing()

set(Headers
  Example.h
)
set(Sources
  Example.cpp
)

add_library(${This} STATIC ${Sources} ${Headers})

add_subdirectory(test)