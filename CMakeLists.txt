cmake_minimum_required(VERSION 3.30)

project(cpp_frame)

set(DEBUG 1)
set(VERSION "0.0.1")
set(MAX_THREADS 5)

set(BUILD_OUTPUT_DIR ${CMAKE_SOURCE_DIR}/build_out)

if(CMAKE_BUILD_TYPE STREQUAL "")
    set(CMAKE_BUILD_TYPE "Debug")
endif()


add_subdirectory(src)