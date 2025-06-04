cmake_minimum_required(VERSION 3.10)

project(SnakeGame)

set(CMAKE_CXX_STANDARD 17)

# Specify the source files
set(SOURCES
    src/main.cpp
    src/game.cpp
)

# Create the executable
add_executable(SnakeGame ${SOURCES})

# Include directories
target_include_directories(SnakeGame PRIVATE src)