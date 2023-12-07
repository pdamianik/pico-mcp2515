set(SUBPROJECT_NAME mcp2515_example)

add_executable(${SUBPROJECT_NAME} pico-mcp2515.cpp)

target_link_libraries(${SUBPROJECT_NAME} pico_stdlib mcp2515)

pico_add_extra_outputs(${SUBPROJECT_NAME})
