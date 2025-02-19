cmake_minimum_required(VERSION 3.10)
project(ChessEngine LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(SOURCE_FILES
    src/main.cpp
)
set(INCLUDE_DIRS include)
add_executable(chess-engine ${SOURCE_FILES})
target_include_directories(chess-engine PRIVATE ${INCLUDE_DIRS})
target_compile_options(chess-engine PRIVATE -Wall -Wextra -Wpedantic)