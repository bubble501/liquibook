
include_directories(${LIQUIBOOK_SOURCE_DIR}/src)
add_library(liquibook simple/simple_order.cpp)

set_property(TARGET liquibook PROPERTY CXX_STANDARD 11)
