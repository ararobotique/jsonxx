cmake_minimum_required(VERSION 3.7)

project(jsonxx)

add_library(jsonxx STATIC
        ${CMAKE_CURRENT_SOURCE_DIR}/jsonxx.cc
        )

target_compile_options(jsonxx PRIVATE -fPIC)

target_include_directories(jsonxx
        PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
        )
