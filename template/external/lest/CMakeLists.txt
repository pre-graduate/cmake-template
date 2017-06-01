include (ExternalProject)

option( LEST_BUILD_TEST    "Build tests for lest" OFF )
option( LEST_BUILD_EXAMPLE "Build examples" OFF )
option( LEST_BUILD_CONTRIB "Build contrib" OFF )

ExternalProject_Add(lest
    PREFIX ${CMAKE_CURRENT_BINARY_DIR}/lest 
    GIT_REPOSITORY "https://github.com/martinmoene/lest"
    GIT_TAG "master"
    INSTALL_COMMAND ""
)

ExternalProject_Get_Property(lest install_dir)

set(LEST_INCLUDE ${install_dir}/src)

message("-- + LEST")