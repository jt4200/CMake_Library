cmake_minimum_required(VERSION "3.16.2")

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib") #set archive targets output dir
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib") #set library targets output dir
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin") #set runtime targets output dir

option(BUILD_SHARED_LIBS "True when building a shared library" TRUE)

project ("Foo")
add_subdirectory("foo")
add_subdirectory("examples")
