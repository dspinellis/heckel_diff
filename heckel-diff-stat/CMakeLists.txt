cmake_minimum_required(VERSION 3.6)

project(heckel-diff-stat)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_CXX_FLAGS_DEBUG  "-O0 -g")
set(CMAKE_CXX_FLAGS_RELEASE "-O3")

add_executable(${PROJECT_NAME} heckel-diff-stat.cpp)

target_link_libraries(${PROJECT_NAME} heckel_diff_lib)

install(TARGETS ${PROJECT_NAME} DESTINATION bin)
