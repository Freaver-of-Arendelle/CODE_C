cmake_minimum_required(VERSION 3.0.0)
project(Signal VERSION 0.1.0)

include(CTest)
enable_testing()

add_library(Signal Signal.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
include_directories(
    /usr/local/include
    /home/arendelle/CODE_C/libs/
)
