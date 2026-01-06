
add_subdirectory(config)

add_subdirectory(xlog)


add_executable(${PROJECT_NAME} main.cc)

target_link_libraries(${PROJECT_NAME} PRIVATE xlog)


include(${CMAKE_SOURCE_DIR}/cmake/common.cmake)
build_output(${PROJECT_NAME})