cmake_minimum_required(VERSION 3.22)

project(compact_vector CXX)

add_library(compact_vector INTERFACE)
target_include_directories(compact_vector INTERFACE include)
target_compile_features(compact_vector INTERFACE cxx_std_11)

if (COMPACT_VECTOR_BUILD_TESTS)
    add_subdirectory(tests)
    add_subdirectory(unittests)
endif()
