cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(hello)

add_executable(hello hello_world.cpp)

add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib ${CMAKE_BINARY_DIR}/formatter_ex_lib)

target_link_libraries(hello formatter_ex)

