cmake_minimum_required(VERSION 3.30)

project(cpp_frame)

include(FetchContent)





set(DPES_DIR ${CMAKE_SOURCE_DIR}/deps/tars)
set(EXTRACT_DIR ${CMAKE_SOURCE_DIR}/deps/extract)
set(BUILD_DEPS_DIR ${CMAKE_BINARY_DIR})

include(${CMAKE_SOURCE_DIR}/cmake/fetchcontent.cmake)
fetch_content(googletest 
    https://github.com/google/googletest/archive/refs/tags/v1.17.0.tar.gz
)

#===================config.h.in===================
set(DEBUG 1)
set(VERSION "0.0.1")
set(MAX_THREADS 5)

set(BUILD_OUTPUT_DIR ${CMAKE_SOURCE_DIR}/build_out)

#==================================================



if(CMAKE_BUILD_TYPE STREQUAL "")
    set(CMAKE_BUILD_TYPE "Debug")
endif()


add_subdirectory(src)