project(Ethernet)

add_library(${PROJECT_NAME} ethernet.cpp)

target_link_libraries(${PROJECT_NAME} ${Boost_LIBRARIES})
