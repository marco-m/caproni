cmake_minimum_required(VERSION 3.9.5)
project(caproni VERSION 0.1 LANGUAGES CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON) # CMake quirk
set(CMAKE_CXX_EXTENSIONS OFF)       # Disable compiler extensions like gnu++11

# find_package()

#
# For this simple project we use only one cmakelist. 
#

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/out)

add_executable(caproni
    src/main.cpp
    src/caproni.cpp)
