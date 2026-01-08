
add_subdirectory(config)

add_subdirectory(xlog)


# add_executable(${PROJECT_NAME} main.cc)

# target_link_libraries(${PROJECT_NAME} PRIVATE xlog)
# build_output(${PROJECT_NAME})

include(${CMAKE_SOURCE_DIR}/cmake/common.cmake)

cc_executable(${PROJECT_NAME} xlog)

