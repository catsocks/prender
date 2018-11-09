cmake_minimum_required(VERSION 2.8)

project(prender C)

find_package(SDL REQUIRED)
include_directories(${SDL_INCLUDE_DIR})

add_executable(${PROJECT_NAME} main.c)

target_link_libraries(${PROJECT_NAME} ${SDL_LIBRARY} m)
