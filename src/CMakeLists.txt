cmake_minimum_required(VERSION 3.2 FATAL_ERROR)

# To allow change `option` by setting variable.
cmake_policy(SET CMP0077 NEW)

set(BUILD_SHARED_LIBS OFF)
set(GLM_TEST_ENABLE_CXX_17 ON)

if(${TEST_DEPENDENCES})
    set(GLM_TEST_ENABLE YES)
else()
    set(GLM_TEST_ENABLE NO)
endif()

add_subdirectory(glm)
