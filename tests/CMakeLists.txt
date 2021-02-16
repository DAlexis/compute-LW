project(lwpc-tests)

set(EXE_SOURCES
    ${PROJECT_SOURCE_DIR}/test-lwpc.cpp
)

add_executable(${PROJECT_NAME} ${EXE_SOURCES} ${EXE_HPP})

target_link_libraries (${PROJECT_NAME} PRIVATE
    gtest
    gtest_main
    lwpc
)

add_test(NAME stmod-testing COMMAND ${PROJECT_NAME})
