cmake_minimum_required(VERSION 3.0.0)

project(main VERSION 0.1.0)

add_subdirectory("./my_library")
add_executable(main main.cpp empty.cpp another_unit.cpp)
target_link_libraries(main PUBLIC my_library)
