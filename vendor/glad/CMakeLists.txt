set(glad_PATH ${CMAKE_CURRENT_SOURCE_DIR})
add_library(glad
        ${glad_PATH}/include/glad/glad.h
        ${glad_PATH}/include/KHR/khrplatform.h
        ${glad_PATH}/src/glad.c
        )

set(GLAD_INCLUDE_DIRS ${glad_PATH}/include PARENT_SCOPE)
set(GLAD_INCLUDE_DIRS ${glad_PATH}/include)

target_include_directories(glad PUBLIC ${GLAD_INCLUDE_DIRS})