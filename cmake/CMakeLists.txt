cmake_minimum_required(VERSION 3.26)
project(space_shooter VERSION 0.1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)

set(SOURCES_DIR ../src)
set(SOURCES_BINARY_DIR ${CMAKE_BINARY_DIR}/bin)
add_subdirectory(${SOURCES_DIR} ${SOURCES_BINARY_DIR})

target_link_options(${PROJECT_NAME} PRIVATE -static)
