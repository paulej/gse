add_executable(test_gs_api test_gs_api.cpp)

include(GoogleTest)

target_link_libraries(test_gs_api PRIVATE gse GTest::GTest GTest::Main)

add_test(NAME test_gs_api
         COMMAND test_gs_api)
