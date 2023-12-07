set(MCP2515_SOURCE ./mcp2515/)

add_library(
    mcp2515 STATIC ${MCP2515_SOURCE}/mcp2515.cpp
)

target_link_libraries(mcp2515 pico_stdlib hardware_spi)

target_include_directories(
    mcp2515 PUBLIC .
)
