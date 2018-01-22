add_definitions(-D_DEFAULT_SOURCE)

add_executable(ouch ouch.c)
target_link_libraries(ouch tlpi)