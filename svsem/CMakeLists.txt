add_executable(svsem_demo svsem_demo.c semun.h)
target_link_libraries(svsem_demo tlpi)

add_executable(svsem_mon svsem_mon.c)
target_link_libraries(svsem_mon tlpi)

add_executable(svsem_setall svsem_setall.c)
target_link_libraries(svsem_setall tlpi)

add_executable(svsem_bad_init svsem_bad_init.c)
target_link_libraries(svsem_bad_init tlpi)

add_executable(svsem_good_init svsem_good_init.c)
target_link_libraries(svsem_good_init tlpi)

add_executable(svsem_op svsem_op.c)
target_link_libraries(svsem_op tlpi)
