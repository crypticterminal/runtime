set(TESTSOURCES
  parentprocess.cpp
)

add_executable(paltest_createprocessa_test2
  ${TESTSOURCES}
)

add_dependencies(paltest_createprocessa_test2 coreclrpal)

target_link_libraries(paltest_createprocessa_test2
  ${COMMON_TEST_LIBRARIES}
)


set(HELPERSOURCES
  childprocess.cpp
)

add_executable(paltest_createprocessa_test2_child
  ${HELPERSOURCES}
)

add_dependencies(paltest_createprocessa_test2_child coreclrpal)

target_link_libraries(paltest_createprocessa_test2_child
  ${COMMON_TEST_LIBRARIES}
)
