cmake_minimum_required(VERSION 3.20)

project(sqlite3)

add_library(sqlite3 SHARED
    src/sqlite3.c src/sqlite3.h
)

add_library(sqlite3_static STATIC
    src/sqlite3.c src/sqlite3.h
)
