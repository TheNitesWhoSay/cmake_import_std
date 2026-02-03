cmake_minimum_required(VERSION 4.2)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_EXPERIMENTAL_CXX_IMPORT_STD "d0edc3af-4c50-42ea-a356-e2862fe7a444")
if ( NOT "${CMAKE_GENERATOR}" MATCHES "Visual Studio.*" )
  set(CMAKE_CXX_MODULE_STD 1)
endif ()

project(import_std)

add_executable(import_std main.cpp)