cmake_minimum_required(VERSION 3.14)
project(projekt3tp VERSION 1.0.0)

add_subdirectory(matplotplusplus)

add_executable(project-base main.cpp)
target_link_libraries(project-base PUBLIC matplot)
