#
#
#

cmake_minimum_required(VERSION 3.5)
project (c_gui)

find_package(GTK2 2.6 REQUIRED gtk)

if(GTK2_FOUND)
  message(STATUS "GTK2_VERSION=${GTK2_VERSION}")
  message(STATUS "GTK2_TARGETS=${GTK2_TARGETS}")
  
  add_executable(f1 src/f1.c)
  target_link_libraries(f1 PRIVATE GTK2::gtk)
  
  add_executable(page81 src/page81.c)
  target_link_libraries(page81 PRIVATE GTK2::gtk)
  
  add_executable(page83 src/page83.c)
  target_link_libraries(page83 PRIVATE GTK2::gtk)
  
  add_executable(page85 src/page85.c)
  target_link_libraries(page85 PRIVATE GTK2::gtk)
  
  add_executable(page87 src/page87.c)
  target_link_libraries(page87 PRIVATE GTK2::gtk)

endif()


