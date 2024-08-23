#
#
#

cmake_minimum_required(VERSION 3.5)
project (c_gui)

SET(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")

find_package(GTK2 2.6 REQUIRED gtk)

add_subdirectory(src)



