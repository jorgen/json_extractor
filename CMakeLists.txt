cmake_minimum_required(VERSION 3.14)
project(json_mod)
set(CMAKE_CXX_STANDARD 11)

find_package (LLVM HINTS $ENV{LLVM_MODULE} REQUIRED)
find_package (Clang HINTS $ENV{LLVM_MODULE} REQUIRED)
add_subdirectory(src)

enable_testing()
add_subdirectory(tests)
