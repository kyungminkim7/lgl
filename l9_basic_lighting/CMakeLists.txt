cmake_minimum_required(VERSION 3.5...3.10)
project(l9_basic_lighting)

add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} lgl::lgl)

configure_file("default.vert" ${CMAKE_CURRENT_BINARY_DIR})
configure_file("default.frag" ${CMAKE_CURRENT_BINARY_DIR})
configure_file("light.frag" ${CMAKE_CURRENT_BINARY_DIR})
