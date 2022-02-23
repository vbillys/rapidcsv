# Project
cmake_minimum_required(VERSION 3.1 FATAL_ERROR)
project(rapidcsv VERSION 1.0 LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 11)

find_package(catkin REQUIRED)

catkin_package(INCLUDE_DIRS src)

# Library
# add_library(rapidcsv INTERFACE)
# target_include_directories(rapidcsv INTERFACE src)

# # Install / Uninstall targets for standalone rapidcsv build
# if(CMAKE_SOURCE_DIR STREQUAL PROJECT_SOURCE_DIR)
#   message(STATUS "Install/uninstall targets enabled.")

#   # Install
#   install(FILES ${CMAKE_CURRENT_SOURCE_DIR}/src/rapidcsv.h DESTINATION include)

#   # Uninstall
#   add_custom_target(uninstall
#                     COMMAND "${CMAKE_COMMAND}" -E remove
#                             "${CMAKE_INSTALL_PREFIX}/include/rapidcsv.h")
# else()
#   message(STATUS "Install/uninstall targets disabled.")
# endif()
