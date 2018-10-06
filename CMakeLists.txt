cmake_minimum_required(VERSION 3.2 FATAL_ERROR)

project(projectname)

set(CMAKE_CXX_STANDARD 17)

file(GLOB SRC
    "src/*.h"
    "src/*.cpp"
)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_BINARY_DIR}/bin)
add_executable(vm ${SRC})

# optionally link libraries
#target_link_libraries(main
#  core)
