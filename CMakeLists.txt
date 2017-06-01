# Minimum version
cmake_minimum_required (VERSION 3.8)

# Set project name
project (CMAKE_TEMPLATE)

# Project Options
option(ENABLE_SAMPLES "Enable Samples" OFF)
option(ENABLE_TESTS "Enable Tests" OFF)

set(CMAKE_MACOSX_RPATH 1)
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_SUPPRESS_REGENERATION true)

# External projects
add_subdirectory(external/lest)

# Our Targets
add_subdirectory(source)

# Add Samples
if(ENABLE_SAMPLES)
    add_subdirectory(samples)
    message(STATUS "Including Samples")
endif()

# Add Tests
if(ENABLE_TESTS)
    add_subdirectory(test)
    message(STATUS "Including Tests")
endif()
