cmake_minimum_required(VERSION 3.15)

project(loader C)
file(GLOB_RECURSE files *.h *.c)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -m32 -std=c99 -w")

add_executable(loader ${files})