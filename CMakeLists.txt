cmake_minimum_required(VERSION 3.17)
project(lab1)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(lib/googletest-master)
include_directories(lib/googletest-master/googletest/include)
include_directories(lib/googletest-master/googlemock/include)

add_executable(lab1 main.cpp tritset.cpp tritset.h tests/tests.cpp)

target_link_libraries(lab1 gtest gtest_main)
