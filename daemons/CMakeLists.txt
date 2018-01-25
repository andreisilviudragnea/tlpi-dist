add_executable(test_become_daemon test_become_daemon.c)
target_link_libraries(test_become_daemon tlpi)

add_executable(daemon_SIGHUP daemon_SIGHUP.c)
target_link_libraries(daemon_SIGHUP tlpi)

add_executable(t_syslog t_syslog.c)
target_link_libraries(t_syslog tlpi)
