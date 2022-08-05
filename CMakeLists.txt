cmake_minimum_required(VERSION 3.15)

project(topk_words LANGUAGES CXX)

find_package(Threads REQUIRED)

add_executable(topk_words main.cpp)

target_link_libraries(topk_words PUBLIC Threads::Threads)

set_target_properties(topk_words PROPERTIES
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED ON
)
