cmake_minimum_required(VERSION 3.5)
project(OpenXLSX.Benchmark)

# C/C++ language version
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(SOURCE_FILES benchmark.cpp table_printer.h)

add_executable(Benchmark ${SOURCE_FILES})
target_link_libraries(Benchmark PUBLIC OpenXLSX)