set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

add_executable(psem_create psem_create.c)
target_link_libraries(psem_create tlpi Threads::Threads)

add_executable(psem_unlink psem_unlink.c)
target_link_libraries(psem_unlink tlpi Threads::Threads)

add_executable(psem_wait psem_wait.c)
target_link_libraries(psem_wait tlpi Threads::Threads)

add_executable(psem_post psem_post.c)
target_link_libraries(psem_post tlpi Threads::Threads)

add_executable(psem_getvalue psem_getvalue.c)
target_link_libraries(psem_getvalue tlpi Threads::Threads)

add_executable(thread_incr_psem thread_incr_psem.c)
target_link_libraries(thread_incr_psem tlpi Threads::Threads)

add_executable(psem_timedwait psem_timedwait.c)
target_link_libraries(psem_timedwait tlpi Threads::Threads)

add_executable(psem_trywait psem_trywait.c)
target_link_libraries(psem_trywait tlpi Threads::Threads)
