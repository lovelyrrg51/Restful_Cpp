cmake_minimum_required(VERSION 3.2.0)
project(Restful_Cpp VERSION 0.1.0)

include(CTest)
enable_testing()

set(CMAKE_CXX_STANDARD 17)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}")

add_subdirectory(dependencies/cpp_redis)
add_subdirectory(dependencies/Crow)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/dependencies/Crow/include)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/dependencies/cpp_redis/includes)

add_executable(cppREST main.cpp)

target_link_libraries(cppREST pthread)
target_link_libraries(cppREST cpp_redis)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
