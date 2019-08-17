cmake_minimum_required(VERSION 3.2 FATAL_ERROR)
project(VulkanTestDependences VERSION 0.0.1 LANGUAGES CXX)

cmake_policy(SET CMP0077 NEW)

option(TEST_DEPENDENCES "Build tests for dependences?" YES)

add_subdirectory(src)
