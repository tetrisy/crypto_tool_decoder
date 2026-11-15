cmake_minimum_required(VERSION 3.16)
project(decoder CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

file(GLOB srcs CONFIGURE_DEPENDS src/*.cpp)

add_executable(decoder ${srcs})
target_include_directories(decoder PRIVATE lib)
