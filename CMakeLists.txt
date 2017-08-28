cmake_minimum_required(VERSION 2.8)
project(LIQUIBOOK)

add_subdirectory(src)
add_subdirectory(test)

enable_testing()

add_test(NAME liquibookTest COMMAND UnitTest)
add_test(NAME perfTest COMMAND PerfTest)
add_test(NAME latencyTest COMMAND LatencyTest)
