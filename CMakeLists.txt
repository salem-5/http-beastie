cmake_minimum_required(VERSION 3.21)
project(Beastie)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Boost REQUIRED)

add_executable(Beastie
        src/main.cpp
        src/utils.cpp
)
target_include_directories(Beastie PRIVATE include)
target_include_directories(Beastie PRIVATE ${Boost_INCLUDE_DIRS})