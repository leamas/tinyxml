cmake_minimum_required(VERSION 3.1.0)

set (SRC
  tinyxml.cpp
  tinyxmlerror.cpp
  tinyxmlparser.cpp
  tinyxml.h
)

add_library(tinyxml SHARED ${SRC})
target_include_directories(tinyxml PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
target_compile_definitions(tinyxml PUBLIC "-DTIXML_USE_STL")
