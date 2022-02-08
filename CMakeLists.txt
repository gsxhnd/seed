cmake_minimum_required(VERSION 3.20)
project(seed)

set(CMAKE_CXX_STANDARD 23)
set(CONAN_DISABLE_CHECK_COMPILER disable)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(seed src/main.cpp)

target_link_libraries(seed ${CONAN_LIBS})