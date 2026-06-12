cmake_minimum_required(VERSION 3.10)
project(VivifyMod)

# This assumes your code is in a folder named 'src'
add_library(VivifyMod SHARED src/main.cpp)

# Quest mods need specific settings
target_include_directories(VivifyMod PUBLIC include)
