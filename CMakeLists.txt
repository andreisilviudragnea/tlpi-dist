cmake_minimum_required(VERSION 3.9)
project(tlpi_dist)

set(CMAKE_C_STANDARD 11)

include_directories(lib)
add_compile_options(-Wall -Wextra -g)

add_subdirectory(lib)
add_subdirectory(signals)