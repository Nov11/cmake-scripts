project(HELLO)
message(${PROJECT_SOURCE_DIR})
message(${PROJECT_BINARY_DIR})
set(SRC_LIST a.cpp )
set(LIB_SRC b.cpp)
add_executable(hello ${SRC_LIST})
add_library(libhello ${LIB_SRC})
target_link_libraries(hello libhello)
