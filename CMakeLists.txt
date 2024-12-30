cmake_minimum_required(VERSION 3.26)
project(lan_core)

add_subdirectory(src)

add_executable(
    lan 
    main.cpp
)

target_include_directories(
    lan
    PRIVATE
    src
)

target_link_libraries(
    lan
    PRIVATE
    hello
)

