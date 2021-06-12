cmake_minimum_required(VERSION 3.1.0)
PROJECT (GTEST)
find_package(GTest REQUIRED)
include_directories(${GTEST_INCLUDE_DIRS})
ADD_EXECUTABLE (gtest gtest.cpp)
target_link_libraries(gtest
	${GTEST_LIBRARY}
	${GTEST_MAIN_LIBRARY}
	pthread)