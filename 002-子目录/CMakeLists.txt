cmake_minimum_required (VERSION 2.8)

project (Test)
add_subdirectory(myLib)
aux_source_directory(. DIR_SRCS)

add_executable(Test main.cpp)
target_link_libraries(Test MyLib)
