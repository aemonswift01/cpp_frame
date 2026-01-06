cmake_minimum_required(VERSION 3.30)

project(cpp_frame)

set(DEBUG 1)
set(VERSION "0.0.1")
set(MAX_THREADS 5)

if(CMAKE_BUILD_TYPE STREQUAL "")
    set(CMAKE_BUILD_TYPE "Debug")
endif()


add_subdirectory(src)