cmake_minimum_required(VERSION 3.10)
project(VivifyMod)

# Include headers for libil2cpp and other Beat Saber internals
include_directories(include)

# Define the library
add_library(${CMAKE_PROJECT_NAME} SHARED
    src/main.cpp
)

# Link against the game's shared libraries
target_link_libraries(${CMAKE_PROJECT_NAME}
    android
    log
    # Add other required libs here
)
