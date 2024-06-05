cmake_minimum_required(VERSION 3.24)

project(CppOpenGLThing)

include(FetchContent)

# FetchContent_Declare(
  # sfml
  # URL https://github.com/SFML/SFML.git
  # GIT_TAG 69ea0cd863aed1d4092b970b676924a716ff718b
# )
# FetchContent_MakeAvailable(sfml)

add_executable(CppOpenGLThing src/main.cpp)

# target_link_libraries(CppOpenGLThing PUBLIC sfml)
