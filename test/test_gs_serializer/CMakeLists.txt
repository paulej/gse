add_executable(test_gs_serializer test_gs_serializer.cpp)

include(GoogleTest)

target_link_libraries(test_gs_serializer PRIVATE gse GTest::GTest GTest::Main)

add_test(NAME test_gs_serializer
         COMMAND test_gs_serializer)
