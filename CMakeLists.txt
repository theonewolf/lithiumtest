cmake_minimum_required(VERSION 3.23.0)
project(hello)

add_definitions("-std=c++17")

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(hello hello.cc)
include_directories(/Users/wolf/Development/include)
target_link_libraries(hello ${CONAN_LIBS})
