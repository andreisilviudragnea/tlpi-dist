add_executable(pshm_create pshm_create.c)
target_link_libraries(pshm_create tlpi Threads::Threads rt)

add_executable(pshm_write pshm_write.c)
target_link_libraries(pshm_write tlpi Threads::Threads rt)

add_executable(pshm_read pshm_read.c)
target_link_libraries(pshm_read tlpi Threads::Threads rt)

add_executable(pshm_unlink pshm_unlink.c)
target_link_libraries(pshm_unlink tlpi Threads::Threads rt)
