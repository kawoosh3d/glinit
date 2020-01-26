cmake_minimum_required(VERSION 3.1)
project(Glad)

add_library(glad /usr/local/include/glad/glad.h /usr/local/src/glad/glad.c)
target_include_directories(glad PUBLIC include/)