cmake_minimum_required(VERSION 3.10)

project(SnakeGame)

set(CMAKE_CXX_STANDARD 17)

# Specify the source files
set(SOURCES
    "04 Snake/main.cpp"
    "04 Snake/game.cpp"
)

# Create the executable
add_executable(SnakeGame ${SOURCES})

# Include directories
include_directories("04 Snake")