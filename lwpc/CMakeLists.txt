cmake_minimum_required(VERSION 3.1)

project(lwpc)

set(LIB_SOURCE
    ${PROJECT_SOURCE_DIR}/lwpc.cpp
    ${PROJECT_SOURCE_DIR}/lwpc.hpp
)

add_library(${PROJECT_NAME} ${LIB_SOURCE})
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_SOURCE_DIR})

set_target_properties(${PROJECT_NAME} PROPERTIES CXX_STANDARD 11)
