# This file is a part of pandas. See LICENSE for details about reuse and
# copyright holders

# Headers: top level
install(FILES
  DESTINATION include/pandas)

#######################################
# Unit tests
#######################################

set(PANDAS_TEST_LINK_LIBS pandas_test_util ${PANDAS_MIN_TEST_LIBS})

ADD_PANDAS_TEST(buffer-test)
ADD_PANDAS_TEST(memory-test)
ADD_PANDAS_TEST(util-test)
