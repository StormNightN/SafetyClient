cmake_minimum_required(VERSION 3.13)
project(SafetyClient)

set(CMAKE_CXX_STANDARD 14)

find_package(OpenSSL REQUIRED)

add_executable(SafetyClient main.cpp)
target_link_libraries(${PROJECT_NAME} OpenSSL::Crypto)