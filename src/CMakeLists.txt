#
#
#

if(GTK2_FOUND)
  message(STATUS "GTK2_VERSION=${GTK2_VERSION}")
  message(STATUS "GTK2_TARGETS=${GTK2_TARGETS}")
  
  add_executable(f1 f1.c)
  target_link_libraries(f1 PRIVATE GTK2::gtk)
  
  add_executable(page81 page81.c)
  target_link_libraries(page81 PRIVATE GTK2::gtk)
  
  add_executable(page83 page83.c)
  target_link_libraries(page83 PRIVATE GTK2::gtk)
  
  add_executable(page85 page85.c)
  target_link_libraries(page85 PRIVATE GTK2::gtk)
  
  add_executable(page87 page87.c)
  target_link_libraries(page87 PRIVATE GTK2::gtk)

endif()

