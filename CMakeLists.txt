cmake_minimum_required(VERSION 3.1)

project(cli VERSION 1.0 LANGUAGES CXX)

find_package(Boost 1.55 REQUIRED COMPONENTS system)
find_package(Threads REQUIRED)

add_library(cli INTERFACE)
target_include_directories(cli INTERFACE include)
target_link_libraries(cli INTERFACE boost_system Threads::Threads)
target_compile_features(cli INTERFACE cxx_std_14)

add_subdirectory(samples)