cmake_minimum_required(VERSION 3.14)
project(Proj2)

set(CMAKE_CXX_STANDARD 17)

include(FetchContent)
FetchContent_Declare(
        prglib
        GIT_REPOSITORY https://github.com/IFSC-Engtelecom-Prg2/Prg2_Trees
        GIT_TAG v1.0.0
)
FetchContent_MakeAvailable(prglib)

include_directories(${prglib_SOURCE_DIR} .)

add_executable(Proj2 main.cpp)

