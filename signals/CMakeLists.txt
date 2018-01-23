add_definitions(-D_DEFAULT_SOURCE)

add_executable(ouch ouch.c)
target_link_libraries(ouch tlpi)

add_executable(intquit intquit.c)
target_link_libraries(intquit tlpi)