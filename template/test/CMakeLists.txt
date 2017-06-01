
include_directories(${LEST_INCLUDE})
include(CTest)

add_executable(tests tests/tests.cpp)
add_test(NAME tests COMMAND tests)

message("adding tests")