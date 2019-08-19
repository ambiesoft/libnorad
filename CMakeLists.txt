# version
cmake_minimum_required(VERSION 3.5.1)

# project name and language
project(libnorad CXX)

# Create lib
add_library(norad norad.cpp)

# Create 'a.out' from 'main.cpp' and 'hello.cpp'
add_executable(testnorad testnorad.cpp)

# link norad when creating testnorad
target_link_libraries(testnorad norad)


