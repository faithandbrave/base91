cmake_minimum_required(VERSION 3.10)
project(base91)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_FLAGS " ${CMAKE_CXX_FLAGS} -pedantic -Wall -Wextra ")

add_executable(base91 base91.cpp)

add_executable(perf_base91 perf_base91.cpp perf_base91.cpp)

add_executable(test_base91 test_base91.cpp test_base91.cpp)

add_test(NAME test_base91 COMMAND test_base91)

enable_testing()

install(TARGETS base91)
