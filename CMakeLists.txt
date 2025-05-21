cmake_minimum_required(VERSION 3.11)

project(rpi-rgb-led-matrix)

add_subdirectory(lib)
add_subdirectory(examples-api-use)
add_subdirectory(utils)

file(WRITE ${PROJECT_BINARY_DIR}/.gitignore
    [=====[
# CMAKE generated file: DO NOT EDIT!
*
*.*
]=====]
)
