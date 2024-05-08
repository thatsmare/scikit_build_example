cmake_minimum_required(VERSION 3.12)
project(projekt3tp VERSION 1.0.0)

include(FetchContent)

FetchContent_Declare(
    matplotplusplus
    GIT_REPOSITORY https://github.com/alandefreitas/matplotplusplus.git
)

FetchContent_MakeAvailable(matplotplusplus)

add_executable(project-base main.cpp)
target_link_libraries(project-base PRIVATE matplotplusplus)