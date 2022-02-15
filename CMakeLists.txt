cmake_minimum_required(VERSION 3.20)
project(alt_project C)

set(CMAKE_C_STANDARD 99)

add_executable(alt_project main.c libs/algorithms/algorithm.c libs/algorithms/algorithm.h libs/algorithms/array/array.c libs/algorithms/array/array.h libs/data_structures/bitset/bitset.c libs/data_structures/bitset/bitset.h)

add_subdirectory(libs)
target_link_libraries(alt_project data_structures)
target_link_libraries(alt_project algorithms)