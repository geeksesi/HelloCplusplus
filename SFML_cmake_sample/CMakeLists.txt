cmake_minimum_required(VERSION 3.1)

project(one)

include_directories(${PROJECT_SOURCE_DIR})
set(EXECUTABLE_NAME "Game")
add_executable(${EXECUTABLE_NAME} src/main.cpp)


find_package(SFML 2.5 COMPONENTS  system window graphics network audio REQUIRED)
target_link_libraries(${EXECUTABLE_NAME} sfml-system sfml-window sfml-graphics sfml-network sfml-audio)
