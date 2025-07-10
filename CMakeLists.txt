cmake_minimum_required(VERSION 3.70)

project(HelloWorld
        VERSION 0.0.1
        DESCRIPTION "Hello World app for Conan test purpose"
        LANGUAGES CXX)

find_package(fmt REQUIRED)

add_executable(${PROJECT_NAME} src/main.cpp)
target_link_libraries(${PROJECT_NAME} PUBLIC fmt::fmt)