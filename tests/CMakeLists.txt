project(BSM)

include(FetchContent)
FetchContent_Declare(googletest URL https://github.com/google/googletest/archive/974e18ee6f146a2418f9cea83170c640e7d622d6.zip)
# For Windows: Prevent overriding the parent project's compiler/linker settings
set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
FetchContent_MakeAvailable(googletest)

add_executable(bsm.test bsm.test.cpp)
target_link_libraries(bsm.test GTest::gtest_main)

include(GoogleTest)
gtest_discover_tests(bsm.test)
