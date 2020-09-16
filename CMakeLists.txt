cmake_minimum_required(VERSION 3.17)
project(Chip-8 VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(SDL2 CONFIG REQUIRED)

add_executable(Chip-8 
	src/main.cpp)
	
target_link_libraries(Chip-8 PRIVATE
	SDL2::SDL2
	SDL2::SDL2main)