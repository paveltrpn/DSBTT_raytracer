cmake_minimum_required(VERSION 3.21)

project (tracer)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON )

file(GLOB TRACER_SRC "src/*.cpp" "src/*.h")
add_executable(tracer)
target_sources(tracer PRIVATE ${TRACER_SRC})
set_target_properties( tracer
    PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY "../bin"
)
