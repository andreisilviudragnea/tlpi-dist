cmake_minimum_required(VERSION 3.9)
project(tlpi_dist)

set(CMAKE_C_STANDARD 11)

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

include_directories(lib)
add_compile_options(
        -Wall
        -Wextra
        -g
        -Wmissing-prototypes
        -Wstrict-prototypes
        -Wmissing-declarations
        -O3
        -flto)

add_subdirectory(lib)
add_subdirectory(daemons)
add_subdirectory(signals)
add_subdirectory(pipes)
add_subdirectory(svsem)
add_subdirectory(psem)
add_subdirectory(pshm)
add_subdirectory(svshm)
