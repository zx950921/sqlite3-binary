cmake_minimum_required(VERSION 3.20)

project(sqlite3)

if(!CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE "Release")
endif()

add_library(sqlite3 SHARED
    src/sqlite3.c
)

add_library(sqlite3_static STATIC
    src/sqlite3.c
)
