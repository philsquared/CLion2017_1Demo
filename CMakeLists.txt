cmake_minimum_required(VERSION 3.6)
project(CLion2017_1Demo)

set(CMAKE_CXX_STANDARD 14)

set(SOURCE_FILES main.cpp CPP17_support/nested_namespaces.cpp)
add_executable(CLion2017_1Demo ${SOURCE_FILES})

add_subdirectory(CPP14_support)
add_subdirectory(CPP17_support)
add_subdirectory(make_auto)
add_subdirectory(precompiled_header)
add_subdirectory(disassembly_debug)
add_subdirectory(catch_test)

# Uncomment this to link the C++14 test lib in
# target_link_libraries( CLion2017_1Demo CPP14_support )