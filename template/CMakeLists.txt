# Minimum version
cmake_minimum_required (VERSION 2.8)

# Set project name
project (CMAKE_TEMPLATE)

set(CMAKE_MACOSX_RPATH 1)
set(CMAKE_CXX_STANDARD 14)

# Add sub projects
add_subdirectory(external)
add_subdirectory(source)
add_subdirectory(test)