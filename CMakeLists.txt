project(stb_image)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}
        ${PROJECT_A_DIRECTORY}/src)

add_library(${PROJECT_NAME}
        STATIC
        stb_image.cpp
        )

target_link_libraries(${PROJECT_NAME}
        PUBLIC
        spdlog
        )

target_include_directories(${PROJECT_NAME}
        PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
        )
