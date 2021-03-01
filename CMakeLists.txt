cmake_minimum_required(VERSION 3.8.0)
project(pluto-engine VERSION 0.0.1)

set(GLFW_INCLUDE_DIR ${CMAKE_SOURCE_DIR}/3rdParty/windows/glfw/include)
set(GLFW_LIB_DIR ${CMAKE_SOURCE_DIR}/3rdParty/windows/glfw/lib)
set(GLFW_LIB_DIRS ${GLFW_LIB_DIR}/glfw3.lib)

add_subdirectory(Editor)