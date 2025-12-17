cmake_minimum_required(VERSION 3.31.6)

project(first VERSION 1.0)

# VERSIONING THE PROJECT
configure_file(firstConfig.h.in firstConfig.h)


add_executable(${PROJECT_NAME} main.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_BINARY_DIR})
