cmake_minimum_required(VERSION 3.4)

project(formatter_ex_lib)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(/../formatter_lib formatter_lib_dir)

add_library(formatter_ex_lib STATIC /formatter_ex.cpp)

target_include_directories(formatter_ex_lib PUBLIC
/../formatter_lib
)

target_link_libraries(formatter_ex_lib formatter_lib)
