cmake_minimum_required(VERSION 3.24)
project(libStNRGen C)

set(CMAKE_C_STANDARD 11)

include_directories(.)
include_directories(include)

add_library(libStNRGen.so SHARED
            src/libstnrgen.c)
add_library(libStNRGen.a STATIC
            src/libstnrgen.c)
