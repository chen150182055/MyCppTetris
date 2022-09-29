cmake_minimum_required(VERSION 3.22)
project(MyCppTetris)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS -lcurses)
message(STATUS "CMAKE_CXX_FLAGS = ${CMAKE_CXX_FLAGS}")
add_executable(MyCppTetris-main MyCppTetris-main.cpp)
add_executable(MyCppTetris MyCppTetris.cpp)
target_link_libraries(MyCppTetris-main curses)
target_link_libraries(MyCppTetris curses)

