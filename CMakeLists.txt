cmake_minimum_required(VERSION 3.1.0 FATAL_ERROR)

project("lwpc-project" CXX)

add_subdirectory(lwpc)
add_subdirectory(3rdparty/googletest)

enable_testing()

add_subdirectory(tests)
