cmake_minimum_required(VERSION 3.2)
project(XTable)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

add_subdirectory(googletest)

include_directories(googletest/include)
link_libraries(gtest)

set(SOURCE_FILES main.cpp)
add_executable(XTable ${SOURCE_FILES})