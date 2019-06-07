project(TestCases)

add_executable(${PROJECT_NAME} test.cpp)

target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_SOURCE_DIR}/src)

target_link_libraries(${PROJECT_NAME} PUBLIC Catch2::Catch2)

add_test(NAME ${PROJECT_NAME} COMMAND ${PROJECT_NAME})
