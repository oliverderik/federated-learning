cmake_minimum_required(VERSION 3.10)

project(federated-learning)

file(GLOB_RECURSE SRC 
        ${PROJECT_SOURCE_DIR}/source/*.cpp)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY build/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY build/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY build/bin)

set (PROJECT_SOURCE_DIR source)

add_executable(federated-learning ${SRC})