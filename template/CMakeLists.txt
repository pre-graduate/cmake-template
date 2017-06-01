# Minimum version
cmake_minimum_required (VERSION 3.8)

# Set project name
project (CMAKE_TEMPLATE)

set(CMAKE_MACOSX_RPATH 1)
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_SUPPRESS_REGENERATION true)

# External projects
add_subdirectory(external/lest)

# Our Targets
add_subdirectory(source)

# Add Tests
add_subdirectory(test)
