cmake_minimum_required(VERSION 3.16)
project(breakout)

find_package(Threads REQUIRED)
#gtkmm
find_check_modules($)
pkg_check_modules( ${GTKMM_LIBRARY_DIRS} )
include_directories( "${GTKMM_INCLUDE_DIRS}")

add_executable(${PROJECT_NAME} main.cpp)