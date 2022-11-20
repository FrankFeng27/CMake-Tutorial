cmake_minimum_required(VERSION 3.10)

project(Tutorial1 VERSION 1.0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

set(CMAKE_GENERATOR_PLATFORM x64)

configure_file(TutorialConfig.h.in TutorialConfig.h)

add_executable(Tutorial1 tutorial.cxx)

target_include_directories(Tutorial1 PUBLIC "${PROJECT_BINARY_DIR}")