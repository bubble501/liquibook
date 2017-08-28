add_executable(LatencyTest lt_order_book.cpp)
include_directories(${LIQUIBOOK_SOURCE_DIR}/src)
target_link_libraries(LatencyTest liquibook)
set_property(TARGET LatencyTest PROPERTY CXX_STANDARD 11)
