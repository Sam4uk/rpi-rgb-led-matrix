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

add_executable(demo demo-main.cc)

target_link_libraries(demo
PRIVATE rgbmatrix
) 

add_executable(input-example input-example.cc)

target_link_libraries(input-example
PRIVATE rgbmatrix
)

add_executable(text-example text-example.cc)

target_link_libraries(text-example
PRIVATE rgbmatrix
)

add_executable(scrolling-text-example scrolling-text-example.cc)

target_link_libraries(scrolling-text-example
PRIVATE rgbmatrix
)

add_executable(clock clock.cc)

target_link_libraries(clock
PRIVATE rgbmatrix
)

add_executable(ledcat ledcat.cc)

target_link_libraries(ledcat
PRIVATE rgbmatrix
)

add_executable(pixel-mover pixel-mover.cc)

target_link_libraries(pixel-mover
PRIVATE rgbmatrix
)