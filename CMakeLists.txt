cmake_minimum_required(VERSION 3.10)

project(project_name)

find_package(CONFIG REQUIRED)

add_executable(project_name src/main.cpp)

target_link_libraries(project_name PRIVATE )
