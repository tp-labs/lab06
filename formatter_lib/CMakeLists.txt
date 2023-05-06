cmake_minimum_required(VERSION 3.4)

project(formatter_lib)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(formatter_lib STATIC ${CMAKE_CURRENT_SOURCE_DIR}/formatter.cpp ${CMAKE_CURRENT_SOURCE_DIR}/formatter.h)
