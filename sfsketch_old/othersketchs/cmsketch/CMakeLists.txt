cmake_minimum_required(VERSION 3.1)
project(cmsketch)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++98")
set(CMAKE_C_FLAGS "-std=c99")

set(SOURCE_FILES BOBHash.cpp cmsketch.cpp)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/bin")

add_executable(cmsketch ${SOURCE_FILES} main.cpp)
