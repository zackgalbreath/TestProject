cmake_minimum_required(VERSION 3.10)
project(TestProject)

include(CTest)

add_executable(good good.cxx)
add_executable(bad bad.cxx)
add_executable(fail fail.cxx)

add_test(NAME fail COMMAND fail)
