find_package (Boost COMPONENTS unit_test_framework REQUIRED)
include_directories(${LIQUIBOOK_SOURCE_DIR}/src
    ${Boost_INCLUDE_DIRS}
    )

add_definitions(-DBOOST_TEST_DYN_LINK)
file(GLOB unittest_files *.cpp)
add_executable(UnitTest ${unittest_files})
# add_executable(UnitTest ut_all_or_none.cpp)
target_link_libraries(UnitTest
    liquibook
    ${Boost_UNIT_TEST_FRAMEWORK_LIBRARY}
    )

set_property(TARGET UnitTest PROPERTY CXX_STANDARD 11)
