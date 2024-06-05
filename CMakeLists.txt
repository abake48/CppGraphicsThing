cmake_minimum_required(VERSION 3.22)

project(CppOpenGLThing)

include(FetchContent)

FetchContent_Declare(
  glfw
  URL https://github.com/glfw/glfw.git
  GIT_TAG 7b6aead9fb88b3623e3b3725ebb42670cbe4c579 
)
FetchContent_MakeAvailable(glfw)

add_executable(CppOpenGLThing src/main.cpp)

target_link_libraries(CppOpenGLThing PUBLIC glfw)

if(BUILDING_TESTS)
  add_subdirectory(test)
endif()
