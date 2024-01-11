cmake_minimum_required(VERSION 3.10)

project(HelloWorldProject)

# Include directories
include_directories(include)

# Define the sources
set(SOURCES
    src/main.cpp
)


# Create the executable
add_executable(helloworld ${SOURCES})
