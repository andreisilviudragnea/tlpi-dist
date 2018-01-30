add_executable(svsem_demo svsem_demo.c semun.h)
target_link_libraries(svsem_demo tlpi)

add_executable(svsem_mon svsem_mon.c)
target_link_libraries(svsem_mon tlpi)

add_executable(svsem_setall svsem_setall.c)
target_link_libraries(svsem_setall tlpi)
