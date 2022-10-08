cmake_minimum_required(VERSION 3.23)
project(Simple_Project)

set(CMAKE_CXX_STANDARD 17)

include_directories(Simple-Output-Project)
add_library(test_library STATIC Simple-Output-Project/output.cpp)

add_executable(Simple_Project main.cpp)


find_library(TEST_LIBRARY test_library lib)
target_link_libraries(Simple_Project LINK_PUBLIC ${TEST_LIBRARY})
