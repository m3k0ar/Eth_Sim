cmake_minimum_required(VERSION 3.13.4)
project(Eth_Sim)

set(CMAKE_CXX_STANDARD 11)

include(CTest)

find_package(Catch2 REQUIRED)
find_package(Boost 1.68 REQUIRED)

add_subdirectory(src)
add_subdirectory(test)

add_executable(Runner main.cpp)

target_include_directories(Runner PUBLIC ${CMAKE_SOURCE_DIR}/src)
