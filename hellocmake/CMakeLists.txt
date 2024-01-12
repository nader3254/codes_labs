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

# Specify the installation path
set(INSTALL_DIR /home/nader/Desktop/ElectroEmbedded/workspace/codes_labs/hellocmake/installdir)

# Install the executable
install(TARGETS helloworld DESTINATION ${INSTALL_DIR}/bin)

# Install the headers
install(DIRECTORY include/ DESTINATION ${INSTALL_DIR}/include)
