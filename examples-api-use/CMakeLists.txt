cmake_minimum_required(VERSION 3.11)

project(examples)

include_directories(
    ../../include
    
    ../include
)

add_executable(minimal-example minimal-example.cc)

target_link_libraries(minimal-example
PRIVATE rgbmatrix
)
