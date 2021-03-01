cmake_minimum_required(VERSION 3.0.0)
project(editor VERSION 0.0.1)

include(CTest)
enable_testing()

message(${GLFW_INCLUDE_DIR})
include_directories(${GLFW_INCLUDE_DIR})
find_package(OpenGL REQUIRED)

add_executable(editor src/main.cpp)

target_link_libraries(editor ${GLFW_LIB_DIRS} OpenGL::GL)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
