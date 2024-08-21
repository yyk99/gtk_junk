#
#
#

cmake_minimum_required(VERSION 3.25)
project (c_gui)

find_package(GTK2 2.6 REQUIRED gtk)

if(GTK2_FOUND)
  include_directories(${GTK2_INCLUDE_DIRS})
  add_executable(f1 src/f1.c)
  target_link_libraries(f1 ${GTK2_LIBRARIES})
endif()


