set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_unit_test(${MERKLECPP_TEST_PREFIX}demo_tree demo_tree.cpp)
add_unit_test(${MERKLECPP_TEST_PREFIX}time_large_trees time_large_trees.cpp)
add_unit_test(${MERKLECPP_TEST_PREFIX}paths paths.cpp)
add_unit_test(${MERKLECPP_TEST_PREFIX}flush flush.cpp)
add_unit_test(${MERKLECPP_TEST_PREFIX}retract retract.cpp)
add_unit_test(${MERKLECPP_TEST_PREFIX}past_root past_root.cpp)
add_unit_test(${MERKLECPP_TEST_PREFIX}serialisation serialisation.cpp)

if(TARGET evercrypt.host)
  add_unit_test(${MERKLECPP_TEST_PREFIX}compare_evercrypt compare_evercrypt.cpp)
endif()
