cmake_minimum_required (VERSION 3.1)
project (project)

set(CMAKE_CXX_STANDARD 20)

include_directories(eigen)
include_directories(googletest)
add_executable(demo demo.cpp)
target_link_libraries(demo gtest_main)
add_test(NAME example_test COMMAND demo)