# ROOT
cmake_minimum_required(VERSION 2.8)

project(IGA)

include (BuildSetup.cmake)
include (BuildFunctions.cmake)

# set (CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})
# set (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})
# set (CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})

set(GED_BRANCH GED_external)
add_subdirectory(GEDLibrary/${GED_BRANCH})
add_subdirectory(IGALibrary)
add_subdirectory(IGAExe)

