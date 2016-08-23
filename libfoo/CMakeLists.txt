cmake_minimum_required(VERSION 3.5)

project (libfoo C)

add_library(foo SHARED impl.c)
target_link_libraries(foo)
install(TARGETS foo LIBRARY DESTINATION lib/)

set(CPACK_GENERATOR "TGZ")
include(CPack)

