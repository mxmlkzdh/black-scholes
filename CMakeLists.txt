cmake_minimum_required(VERSION 3.26.2)
project(BSM VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_compile_options($<$<CONFIG:Debug>:-Wsign-conversion>)
add_compile_options($<$<CONFIG:Debug>:-Wall>)
add_compile_options($<$<CONFIG:Debug>:-Wextra>)
add_compile_options($<$<CONFIG:Debug>:-Wpedantic>)

add_executable(main examples/main.cpp)

include_directories("include")
include_directories("external")

include(CTest)
enable_testing()
add_subdirectory("tests")