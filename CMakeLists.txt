cmake_minimum_required(VERSION 3.10)

# set the project name
project(CMakeTest)

# add the executable
add_executable(Main Main.c)

#Tests
enable_testing()

add_test(NAME test COMMAND Main)
set_tests_properties(test PROPERTIES PASS_REGULAR_EXPRESSION "Hello World!")
