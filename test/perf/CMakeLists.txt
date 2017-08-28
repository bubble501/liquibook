add_executable(PerfTest pt_order_book.cpp)
include_directories(${LIQUIBOOK_SOURCE_DIR}/src)
target_link_libraries(PerfTest liquibook)
set_property(TARGET PerfTest PROPERTY CXX_STANDARD 11)
