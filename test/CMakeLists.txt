
add_executable(test test.cpp)

set_target_properties(test PROPERTIES RUNTIME_OUTPUT_DIRECTORY "${PROJECT_BINARY_DIR}")

target_include_directories(test PRIVATE ${PROJECT_SOURCE_DIR}/include)

target_link_libraries(test figtree)

add_dependencies(test figtree)