cmake_minimum_required(VERSION 3.4)
project(design_pattern_in_modern_cpp)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

macro(add_example name)
  add_executable(${name} ${name}.cpp)
endmacro()

add_subdirectory(Behavioral)
add_subdirectory(Creational)
add_subdirectory(Structural)
