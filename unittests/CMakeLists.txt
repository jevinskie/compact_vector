find_package(GTest REQUIRED)

add_executable(test_compact_vector test_compact_vector.cc test_dyn.cc test_stat.cc)
target_link_libraries(test_compact_vector compact_vector GTest::gtest GTest::gtest_main)
