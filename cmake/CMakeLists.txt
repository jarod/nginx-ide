# https://cmake.org/cmake/help/latest/
project(nginx-ide C)
cmake_minimum_required(VERSION 2.4)
set(ROOT_DIR "${PROJECT_SOURCE_DIR}/..")
add_subdirectory(nginx)
add_subdirectory(nginx-rtmp-module)
