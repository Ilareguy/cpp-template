cmake_minimum_required(VERSION 3.8)
project(cpp-template)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
message(STATUS "Using toolchain file: ${CMAKE_TOOLCHAIN_FILE}.")

add_executable(program
        src/main.cpp)
