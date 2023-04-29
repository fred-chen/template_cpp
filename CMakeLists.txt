cmake_minimum_required(VERSION 3.0.0)
project(template_cpp VERSION 0.1.0)

include(CTest)
enable_testing()

include_directories(include)

set(SRCDIR src)
add_executable(template_cpp ${SRCDIR}/main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
