cmake_minimum_required(VERSION 3.19)
project(automata_by_regexp)

set(CMAKE_CXX_STANDARD 14)

include_directories(include)

aux_source_directory(src SRC)

add_executable(test test/test-aut.cpp
        ${SRC}
        )