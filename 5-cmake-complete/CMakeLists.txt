cmake_minimum_required(VERSION 3.10)

project(helloworld)

set(VERSION 1.0.0)

message("Building ${CMAKE_PROJECT_NAME}")

list(APPEND SRC main.c)  # i.e. SRC.push_back("main.c")

add_executable(${CMAKE_PROJECT_NAME} ${SRC})
