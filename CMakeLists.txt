cmake_minimum_required(VERSION 3.10)

project(SnakeGame)

set(CMAKE_CXX_STANDARD 17)

# Specify the source files
set(SOURCES
    "04 Snake/main.cpp"
)

# Create the executable
add_executable(SnakeGame ${SOURCES})

# Rename output executable
set_target_properties(SnakeGame PROPERTIES OUTPUT_NAME "snake-game")

# Include directories
include_directories("04 Snake")

# Add images directory
file(COPY "04 Snake/images" DESTINATION "${CMAKE_BINARY_DIR}")

find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

# Link SFML libraries
target_link_libraries(SnakeGame sfml-graphics sfml-window sfml-system)