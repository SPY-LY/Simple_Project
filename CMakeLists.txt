cmake_minimum_required(VERSION 3.23)
project(Simple_Project)

set(CMAKE_CXX_STANDARD 14)

include_directories(Simple-Output-Project)

add_executable(Simple_Project
        Simple-Output-Project/CMakeLists.txt
        main.cpp)
