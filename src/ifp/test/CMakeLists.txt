# Copyright 2022 Google LLC
#
# Use of this source code is governed by a BSD-style
# license that can be found in the LICENSE file or at
# https://developers.google.com/open-source/licenses/bsd

include("openroad")

add_executable(ifp_test ifp_test.cc)

target_link_libraries(ifp_test 
    GTest::gtest 
    GTest::gtest_main
    ifp
)

gtest_discover_tests(ifp_test)

