
# Include LEST for unit tests
include_directories(${LEST_INCLUDE})

# Add test executable and mark as a test to cmake
add_executable(test01 test01/main.cpp)
add_test(NAME test01 COMMAND test01)
