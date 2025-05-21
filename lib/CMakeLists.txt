cmake_minimum_required(VERSION 3.11)

project(rgbmatrix)

include_directories(
    ../include
)

add_library(rgbmatrix
    led-matrix.cc
    graphics.cc
    led-matrix.cc
    thread.cc
    framebuffer.cc
    graphics.cc
    gpio.cc
    hardware-mapping.c
    options-initialize.cc
    multiplex-mappers.cc
    pixel-mapper.cc
    bdf-font.cc
)