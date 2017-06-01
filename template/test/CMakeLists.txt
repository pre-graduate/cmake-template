
include_directories(${LEST_INCLUDE})
include(CTest)

add_executable(basic-tests basic/basic.cpp)
add_test(NAME basic-tests COMMAND basic-tests)
