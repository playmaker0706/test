cmake_minimum_required(VERSION 3.26)
project(hello)

add_library(hello SHARED)

target_sources(hello PRIVATE hello.cpp) 

set_target_properties(hello PROPERTIES
    OUTPUT_NAME hello
)
