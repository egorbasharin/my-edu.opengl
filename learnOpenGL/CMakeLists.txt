cmake_minimum_required(VERSION 3.17)
project(learnOpenGL)

set(CMAKE_CXX_STANDARD 17)

include_directories(include)
include_directories(/usr/local/include)

link_directories(/usr/local/lib)

add_executable(learnOpenGL src/main.cpp src/glad.c)

target_link_libraries(learnOpenGL glfw3)
target_link_libraries(learnOpenGL "-framework Cocoa")
target_link_libraries(learnOpenGL "-framework OpenGL")
target_link_libraries(learnOpenGL "-framework IOKit")
