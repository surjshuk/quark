# Minimum CMake version required
cmake_minimum_required(VERSION 3.10)

# Project name and version
project(Quark VERSION 0.1)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Specify the source files
set(SOURCES
    src/main.cpp
)

# Add the executable
add_executable(Quark ${SOURCES})

# Include header directories
target_include_directories(Quark PUBLIC include)

# Print message to confirm build configuration
message("Building Quark: Hello World!")

